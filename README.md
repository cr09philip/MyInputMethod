# MyInputMethod
MyInputMethod一款iOS上的第三方输入法。集拼音,五笔,笔画,快捷短语/emoji/emoticon/图片表情/符号/上滑/左滑/粘贴等输入方式,及英文补全,自定义皮肤/样式等功能... http://app.wodedata.com

## 技术参考:

iOS基础集合类:[https://github.com/ming1016/study/wiki/iOS%E5%9F%BA%E7%A1%80%E9%9B%86%E5%90%88%E7%B1%BB](https://github.com/ming1016/study/wiki/iOS%E5%9F%BA%E7%A1%80%E9%9B%86%E5%90%88%E7%B1%BB)

iOS-Core-Animation-Advanced-Techniques:[http://www.cocoachina.com/ios/20150104/10814.html](http://www.cocoachina.com/ios/20150104/10814.html)

自定义控件:[http://objccn.io/issue-3-4/](http://objccn.io/issue-3-4/)

How To Make a Custom Control:[http://www.raywenderlich.com/36288/how-to-make-a-custom-control](http://www.raywenderlich.com/36288/how-to-make-a-custom-control)

AutoLayoutDemo:[https://github.com/yechunjun/AutoLayoutDemo](https://github.com/yechunjun/AutoLayoutDemo)

先进的自动布局工具箱:[http://objccn.io/issue-3-5/](http://objccn.io/issue-3-5/)

细数AutoLayout以来UIView和UIViewController新增的相关API:[http://chun.tips/blog/2014/10/23/xi-shu-autolayoutyi-lai-uiviewhe-uiviewcontrollerxin-zeng-de-xiang-guan-api-uiviewpian/](http://chun.tips/blog/2014/10/23/xi-shu-autolayoutyi-lai-uiviewhe-uiviewcontrollerxin-zeng-de-xiang-guan-api-uiviewpian/)

自动布局（autolayout）环境下图片编辑器的实现:[http://blog.csdn.net/lihuiqwertyuiop/article/details/40015521](http://blog.csdn.net/lihuiqwertyuiop/article/details/40015521)

iOS界面开发的大一统:[http://onevcat.com/2014/07/ios-ui-unique/](http://onevcat.com/2014/07/ios-ui-unique/)

How can I set image in textDocumentProxy with custom keyboard extension iOS 8?:[http://stackoverflow.com/questions/28630338/how-can-i-set-image-in-textdocumentproxy-with-custom-keyboard-extension-ios-8](http://stackoverflow.com/questions/28630338/how-can-i-set-image-in-textdocumentproxy-with-custom-keyboard-extension-ios-8)

iOS-Headers私有API:[https://github.com/MP0w/iOS-Headers](https://github.com/MP0w/iOS-Headers)

Undo typing in UITextView:[http://stackoverflow.com/questions/1991897/undo-typing-in-uitextview](http://stackoverflow.com/questions/1991897/undo-typing-in-uitextview)

Undo/redo with a UITextView:[http://stackoverflow.com/questions/4070291/undo-redo-with-a-uitextview-ios-iphone/4071681#4071681](http://stackoverflow.com/questions/4070291/undo-redo-with-a-uitextview-ios-iphone/4071681#4071681)

Designing for iOS - Taming UIButton:[https://robots.thoughtbot.com/designing-for-ios-taming-uibutton](https://robots.thoughtbot.com/designing-for-ios-taming-uibutton)

加密你的SQLite:[http://foggry.com/blog/2014/05/19/jia-mi-ni-de-sqlite](http://foggry.com/blog/2014/05/19/jia-mi-ni-de-sqlite)

纯UILabel实现文字的竖排显示:[http://humin.me/archives/68](http://humin.me/archives/68)

make a vertical text UILabel and UITextView for iOS:[http://stackoverflow.com/questions/28544714/how-do-you-make-a-vertical-text-uilabel-and-uitextview-for-ios-in-swift](http://stackoverflow.com/questions/28544714/how-do-you-make-a-vertical-text-uilabel-and-uitextview-for-ios-in-swift)

Vertical-Text-iOS:[https://github.com/sangonz/Vertical-Text-iOS](https://github.com/sangonz/Vertical-Text-iOS)

Method Swizzling 和 AOP 实践:[http://tech.glowing.com/cn/method-swizzling-aop/](http://tech.glowing.com/cn/method-swizzling-aop/)


## 资源参考：

### 特殊符号:
Unicode字符:[https://en.wikipedia.org/wiki/Category:Unicode](https://en.wikipedia.org/wiki/Category:Unicode)

### 特殊表情:
getEmoji:[http://getemoji.com/](http://getemoji.com/)

Unicode/List of useful symbols:[https://en.wikibooks.org/wiki/Unicode/List_of_useful_symbols](https://en.wikibooks.org/wiki/Unicode/List_of_useful_symbols)

Emoji Unicode Tables:[http://apps.timwhitlock.info/emoji/tables/unicode](http://apps.timwhitlock.info/emoji/tables/unicode)


### 词库
五笔编码词库:[https://github.com/ishitcno1/googleInputWubiTable](https://github.com/ishitcno1/googleInputWubiTable)


### 汉字转拼音:
[https://github.com/jifei/Pinyin/](https://github.com/jifei/Pinyin/)

[https://github.com/cleverdeng/pinyin.py](https://github.com/cleverdeng/pinyin.py)

### 手写识别：
一个iOS版的基于zinnia的手写汉字识别:[https://github.com/Crazylitm/HZRC](https://github.com/Crazylitm/HZRC)

## 实现的功能需求点

### 键盘Extension
**Part 1**
```
1. 自定义皮肤,按键样式设置完善及数据存储整理；
2. 四种常规键盘(拼音全键,拼音九键,五笔全键,笔画全键)之间切换，上滑手势输入，字符键按提示窗；
3. 添加符号键盘(类似百度的符号键盘-CollectionView)；
4. 五种特殊键盘(快捷短语/emoji/emoticon/图片表情/符号键盘)
    1. 数据源统一改成plist文件存储;
    2. 添加常用分类并存储到对应plist文件；
    3. 排序的优化；
5. 主设置界面修改及存储；
6. 输入候选区的添加；
7. 英文补全；
8. 繁简转换；
9. 火星文字转换；
10. 拼音全键输入实现；
11. 拼音九键输入实现；
12. 五笔全键输入实现；
13. 笔画全键输入实现；
14. 输入加入联想联系人逻辑；
15. 九种键盘的删除键/空格键长按输入；
16. 横竖屏优化,剪粘板,按键音处理；
17. 图片表情的社会化分享的集成；
18. 主题的添加/设置/选择；
```

**Part 2(已完成)**
```
1. 修改样式及时生效,及皮肤设置长按恢复默认样式；
2. 许多不使用键盘默认变为拼音全键盘bug；
3. enter键长按：换行功能；
4. 切换键盘或地球键长按/短按 - 英文输入词上屏；
5. 五笔一/二/三/四级简码词频设置；
6. 自定义添加大图片表情；
7. 加载图片选择器时，释放词库；
8. 自定义短语添加(主App)；
9. 默认主题；
10. 搜索：百度及网易云音乐；(入口：光标滑动的长按弹出搜索栏；logo菜单；地球键；)
11. 涂鸦：(入口：表情长按；logo菜单；地球键；)
12. 翻译:(入口：搜索工具栏上翻译按钮；logo菜单；地球键)
13. 联系人名片：(入口：快捷短语添加一个分类按钮，logo菜单)
14. 拼音注音转换：(入口：logo菜单；收起键盘键长按)
15. 密文处理：(入口：表情长按)
16. 相册、联系人选择：(入口：搜索弹窗；logo菜单)；
17. 手写输入(通过使用在线web api方式实现)；
18. 添加快捷短语及分类；
19. 图片表情的添加及分类；
```

**Part 3(已完成)**
```
1. 长按加密聊天；
2. 直接http url -> 打开web页，刷新、分享、收藏下载图片，Safari打开；
3. 毛笔书写；
4. GIF分类搜索；
5. 样式设置顺序调整；
6. 表情分类顺序调整、可编辑；
7. 手写板遮罩层；
8. Web的404页面及弹窗处理；
9. 键间距配置；
10. 音乐搜索限制；
11. 分享面板QQ，微信是否安装检查；
12. sqlite加密；
13. 背景色与PopView颜色互换，搜索、翻译、拼音背景色调整；
14. 保存到相册权限判断，翻译模式下，长按候选词逻辑；
15. 符号及表情类型最近使用的分类记忆；
16. 二维码截图分享默认截取区域修改；
17. 服务端增加禁用开关；
18. 网络不通时打开Web搜索阻塞主UI;
19. 九宫格拼音更多候选词展示问题；
20. 资源本地化及主App数据网络请求；
```

**主App(已完成)**
```
1. 输入法教程Guide；
2. 五笔输入指南(百度文库资料)：
    1. 五笔字根表；
    2. 五笔各级简码指南；(https://wenku.baidu.com/view/42504df17c1cfad6195fa7c5.html)
    3. 特殊词编码分类；
3. 笔划输入指南:https://wenku.baidu.com/view/f53654286edb6f1aff001f3b.html
4. 背景图模糊度调节；
5. 关于&源码；
6. 主App无网络的情况下的处理；
7. 首页中部Logo文字用物理摔子替代；
8. WKWebView 404页面问题修改；
9. 完善App画板；
10. 主App图片增加保存,Detail页增加分享,跳safari,同样键盘网页都可跳过来；
11. 留言反馈；
12. 小工具Google Web 翻译；
13. 小工具Baidu原生页翻译；
14. 小工具拼音转换；
15. 二维码生成器；
16. 小工具二维码扫描及生成；
17. 远程推送打开指定落地页；
18. 小工具建桌面快捷方式；
19. 小工具App高级涂鸭板与键盘涂鸭关联映射；
20. 主App分享加入微博，分享标识为万能输入法App；
21. 第三方应用打开网页直接跳到App对应页或提示安装。
22. 打包记得把几个库改用为Release版本的；
23. 分享：微信好友、收藏、朋友圈、QQ、系统、Safari打开；
```


## 后续优化需求点

**键盘Extension**
```
1. 动画的添加；
2. 边缘上滑展开、下滑折叠手势；
3. 英文常用url词库补全；
4. 点击统计；
```
**工具栏按钮长按响应规则**
```
1. logo长按弹起聊天窗；
2. 光标滑动的长按弹出搜索栏；
3. 收起键盘键长按拼音转换；
```

**主App**
```
1. 小工具喝水提醒；
2. 小工具语音备忘每日一记；
3. 小工具卡密管理,sqlite；
4. 小工具音乐播放；
5. 小工具直播，IM聊天；
6. 小工具成语正则搜索；
7. 联系人的导入；
8. 不同输入框类型测试;
9. Gif图片大小帧率处理
10. live photos转Gif导入；
11. gif图片/压缩包的导入；
12. url下载gif导入；
13. 恢复到默认主题设置；
14. 第三方App分享图片到表情的Share Extension;
```


## 部分API分享

### 百度翻译API
[http://api.fanyi.baidu.com/api/trans/product/desktop?req=developer](http://api.fanyi.baidu.com/api/trans/product/desktop?req=developer)

### 网易云音乐分析

**搜索歌曲**
```
curl --request POST \
  --url http://music.163.com/api/search/get \
  --header 'content-type: application/x-www-form-urlencoded' \
  --header 'referer: http://music.163.com/' \
  --data 's=%E6%BC%94%E5%91%98&type=1&offset=0&total=true&limit=20'
```

**歌曲详情**
```
curl --request GET \
  --url 'http://music.163.com/api/song/detail/?id=32507038&ids=%5B32507038%5D' \
  --header 'referer: http://music.163.com/'
```

**音乐文件下载地址**
```
import md5

def encrypted_id(id):
    byte1 = bytearray('3go8&$8*3*3h0k(2)2')
    byte2 = bytearray(id)
    byte1_len = len(byte1)
    for i in xrange(len(byte2)):
        print i,    # print 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15
        byte2[i] = byte2[i]^byte1[i%byte1_len]
    m = md5.new()
    # str2 = "".join(map(chr, byte2))
    m.update(str(byte2))
    result = m.digest().encode('base64')[:-1]
    print result    # print WddsKHFgZv5+uS8mXxREcA==
    result = result.replace('/', '_')
    result = result.replace('+', '-')
    return result

print(encrypted_id('3233663700533995'))     # print WddsKHFgZv5-uS8mXxREcA==

for i in xrange(10):
    print i,

print 'test\n'[:-1] # delete last charater

a=range(10)
print a         # print [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print a[:-1]    # print [0, 1, 2, 3, 4, 5, 6, 7, 8]
```

#### 参考
**网易云音乐API分析**
[](https://github.com/yanunon/NeteaseCloudMusic/wiki/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90API%E5%88%86%E6%9E%90)

**网易云音乐的API**
[https://zhuanlan.zhihu.com/p/21326015](https://zhuanlan.zhihu.com/p/21326015)

**网易云音乐新版WebAPI分析**
[https://github.com/darknessomi/musicbox/wiki/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90%E6%96%B0%E7%89%88WebAPI%E5%88%86%E6%9E%90%E3%80%82](https://github.com/darknessomi/musicbox/wiki/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90%E6%96%B0%E7%89%88WebAPI%E5%88%86%E6%9E%90%E3%80%82)

**网易云音乐常用API浅析**
[http://moonlib.com/606.html](http://moonlib.com/606.html)

**网易云音乐API**
[http://www.jianshu.com/p/ab746499b920](http://www.jianshu.com/p/ab746499b920)

**网易云音乐api整理（神坑慎入）**
[http://qianzewei.com/2015/12/10/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90api%E6%95%B4%E7%90%86/](http://qianzewei.com/2015/12/10/%E7%BD%91%E6%98%93%E4%BA%91%E9%9F%B3%E4%B9%90api%E6%95%B4%E7%90%86/)


## mac输入法相关资料

[OpenVanilla 輸入法套件](https://github.com/openvanilla/openvanilla)

[OpenVanilla輸入法框架官网](https://openvanilla.org/)

[Input Method Kit Framework Reference](https://developer.apple.com/reference/inputmethodkit)

[NumberInput_IMKit_Sample](https://developer.apple.com/library/content/samplecode/NumberInput_IMKit_Sample/Introduction/Intro.html#//apple_ref/doc/uid/DTS40007466)

[ Apple's NumberInput sample code with each 'step' commit](https://github.com/pkamb/NumberInput_IMKit_Sample)

[InputMethodKit reference](https://developer.apple.com/search/?q=InputMethodKit)

[A better input source switcher for OS X](https://github.com/noraesae/kawa)

[Rime Input Method Engine, the core librar](https://github.com/rime/librime)

[现在如何在 Mac OS X 中写一套输入法 (一)](http://blog.jjgod.org/2007/05/11/write-an-im-in-osx-now/)

[OS X Yosemite: 创建和使用您自己的输入源](https://support.apple.com/kb/PH18456?locale=zh_CN)


## 其他

**Google Cloud Platform**
[https://cloud.google.com/appengine/docs/python/endpoints/consume_ios#adding_a_sign-in_dialog_to_your_ios_client](https://cloud.google.com/appengine/docs/python/endpoints/consume_ios#adding_a_sign-in_dialog_to_your_ios_client)

**百度汉语：**[http://hanyu.baidu.com/](http://hanyu.baidu.com/)

**书法字典**

[墨客书法在线字典](http://zd.shufa99.com)

[书法字典在线查询](http://www.9610.com/zidian/)

[墨客书法字典](http://m.shufa99.com/)

[中国书法网](http://www.shufa.com/zd/)

**中文字码转换**
[中文码表查询](https://github.com/mahiuchun/zh-hk)


**voice over**
[支持voice over](http://www.jianshu.com/p/c793477d021b)

**Markdown/网址撰写模式**
Markdown撰写模式：[MXMarkdownKeyboard](https://github.com/mexiQQ/MXMarkdownKeyboard)


**推送测试**
使用工具NWPusher测试更方便：[https://github.com/noodlewerk/NWPusher](https://github.com/noodlewerk/NWPusher)

```Json
{
  "aps": {
    "alert": "维维维维维维维维维维维维维维维维",
    "badge": 1,
    "sound": "default"
  },
  "url":"LWInputMethod://home.https?url=https%3a%2f%2fm.baidu.com"
}
```


