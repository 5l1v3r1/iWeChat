![](https://github.com/lefex/iWeChat/blob/master/image/bannel.png?raw=true)



- [🐶初衷](https://github.com/lefex/iWeChat#%E5%88%9D%E8%A1%B7)

- [🐱APP信息](https://github.com/lefex/iWeChat#app%E4%BF%A1%E6%81%AF)
  - [💯砸壳 - ipa 获取](https://github.com/lefex/iWeChat#app%E4%BF%A1%E6%81%AF)
  - [💯头文件](https://github.com/lefex/iWeChat#%E5%A4%B4%E6%96%87%E4%BB%B6)
  - [💯第三方库](https://github.com/lefex/iWeChat#%E7%AC%AC%E4%B8%89%E6%96%B9%E5%BA%93)
  - [💯UI](https://github.com/lefex/iWeChat#ui)
  - [💯继承层级](https://github.com/lefex/iWeChat#%E7%BB%A7%E6%89%BF%E5%B1%82%E7%BA%A7)
  - [💯数据库设计](https://github.com/lefex/iWeChat#%E6%95%B0%E6%8D%AE%E5%BA%93%E8%AE%BE%E8%AE%A1)
  - [💯沙盒目录](https://github.com/lefex/iWeChat#%E6%B2%99%E7%9B%92%E7%9B%AE%E5%BD%95)
  - [💯Pod 集成](https://github.com/lefex/iWeChat#pod-%E9%9B%86%E6%88%90)
  - [💯查看网络请求数据](https://github.com/lefex/iWeChat#%E6%9F%A5%E7%9C%8B%E7%BD%91%E7%BB%9C%E8%AF%B7%E6%B1%82%E6%95%B0%E6%8D%AE)

- [🐰工具使用说明](https://github.com/lefex/iWeChat#%E5%B7%A5%E5%85%B7%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E)
  - [💯CaptainHook Hook 代码]()
  - [💯Logos 语法](https://github.com/lefex/iWeChat#logos-%E8%AF%AD%E6%B3%95)
  - [💯查找可执行文件技巧](https://github.com/lefex/iWeChat#%E6%9F%A5%E6%89%BE%E5%8F%AF%E6%89%A7%E8%A1%8C%E6%96%87%E4%BB%B6%E6%8A%80%E5%B7%A7)

- [🐼业务逻辑](https://github.com/lefex/iWeChat#%E4%B8%9A%E5%8A%A1%E9%80%BB%E8%BE%91)
  - [💯还原某些UI的设计](https://github.com/lefex/iWeChat#%E8%BF%98%E5%8E%9F%E6%9F%90%E4%BA%9Bui%E7%9A%84%E8%AE%BE%E8%AE%A1)
  - [💯探索各个模块业务逻辑](https://github.com/lefex/iWeChat#%E6%8E%A2%E7%B4%A2%E5%90%84%E4%B8%AA%E6%A8%A1%E5%9D%97%E4%B8%9A%E5%8A%A1%E9%80%BB%E8%BE%91)
  - [💯消息类型](https://github.com/lefex/iWeChat#%E6%B6%88%E6%81%AF%E7%B1%BB%E5%9E%8B)
  - [💯文件说明](https://github.com/lefex/iWeChat#%E6%96%87%E4%BB%B6%E8%AF%B4%E6%98%8E)

- [🦁错误总结](https://github.com/lefex/iWeChat#%E9%94%99%E8%AF%AF%E6%80%BB%E7%BB%93)

- [🙈相关推荐](https://github.com/lefex/iWeChat#%E5%A5%BD%E6%96%87%E6%8E%A8%E8%8D%90)

- [🐯联系信息](https://github.com/lefex/iWeChat#%E8%81%94%E7%B3%BB%E4%BF%A1%E6%81%AF)

## 🐶初衷

**我们一起还原微信，探索微信的奥妙之处**。微信作为 IM 领域的佼佼者，更是 APP 中的翘楚。它里面有很多值得开发者借鉴的地方，小到某个 View 的设计，大到整个APP的架构，一系列隐藏在背后的技术手段或交互设计需要我们挖掘。所以，希望通过 iWeChat 这个项目能够勾勒出微信的设计，使用到的技术手段等。最重要的是，从这个项目中，你可以学到如何分析一个第三方 APP。

## 🐱APP信息

#### 💯砸壳 - ipa 获取

首先第一步是获取一个破解的 ipa 包，我们可以通过下面这几种方式获取：

- 方式一：iTunes

苹果既然在高版本的 iTunes 取消了获取 ipa 包的入口，那我们就想办法降级处理。需要下载低版本的 iTunes。 [下载](http://secure-appldnld.apple.com/itunes12/091-33628-20170922-EF8F0FE4-9FEF-11E7-B113-91CF9A97A551/iTunes12.6.3.dmg)。

下载完后，安装，第一次启动的时候按住 option 键，这样才不会报错，安装完成后，即可下载应用的 ipa 包。下载完成后，在应用的图标上按右键，show in finder 即可找到 ipa 包。

![](https://github.com/awesome-tips/iOS-Tips/blob/master/images/2018/06/4-1.jpg)

- 方式二：pp助手

电脑安装一个 pp助手客户端，直接下载越狱应用，下载完成后，即可在“本地应用”中找打 APP 的 ipa 包。需要强调一点，这种方式下载的应用是解密后的 ipa。

![](https://github.com/awesome-tips/iOS-Tips/blob/master/images/2018/06/4-2.jpg)

- 方式三：抓包

在 Mac 中的 iTunes 中下载应用，通过 Charles 抓包获取到 ipa 包的下载地址，直接在浏览器中下载，下载地址是在 p52-buy.itunes 这个域名下。

获取到 ipa 包后就需要砸壳。如果从越狱助手上下载的则不需要砸壳。

#### 💯头文件

**头文件导出**

> This is a command-line utility for examining the Objective-C runtime information stored in Mach-O files. It generates declarations for the classes, categories and protocols. This is the same information provided by using ‘otool -ov’, but presented as normal Objective-C declarations, so it is much more compact and readable.


[class-dump](https://github.com/nygard/class-dump) 这个工具用来查看某个APP的头文件。只需要找到第三方APP的 xxx.app 文件，然后执行 class-dump 命令即可。不过在执行 class-dump 命令前，需要确保 xxx.app 是砸过壳的，从 APPStore下载的 xxx.app 文件是经过加密处理的，可以直接从各大越狱市场上下载第三方 xxx.app 文件，从越狱市场下载的 xxx.app 已被破解。可以直接使用 class-dump 导出头文件。



下载 class-dump 后把 class-dump 导入 `/usr/local/bi` 目录下，并执行下列命令：

```
sudo chmod 777/usr/local/bin/class-dump
```

执行 class-dump 命令：

```
class-dump -H [xxx.app所在的位置] -o [头文件导出的位置]

比如：
class-dump -H Lefex.app -o lefexheader

class-dump -H /Users/daredos/Desktop/微信-6.3.23\(越狱应用\)/Payload/WeChat.app  -o /Users/daredos/Desktop/w
```

使用 class-dump 命令导出头文件有以下特点：

- 不管 .h 还是 .m 文件中的属性和方法都会被导出；
- 某个类的类别中的方法也会被导出，导出到源文件中，比如 ViewController (Navigation) 中的方法被导出到 ViewController 中；
- 实现的协议也会被导出，比如 ViewControllerDelegate 的方法被导出到 ViewController 中，如果 ViewController 不实现 ViewControllerDelegate 协议讲不会被导出；
- 协议中定义的方法不会被导出，只会导出到实现协议的类中；

**头文件分类**

有时候为了分析方便，需要把所有的头文件分成不同的文件夹存放。也就是说把他组织成我们开发 APP 时的目录结构。而微信的目录结构大致如下：

把头文件按模块来划分，最后能勾勒出微信的整体项目结构放到主工程中。目前已经勾勒出微信的目录结构，不过不是很全。[参考](https://everettjf.com/2016/11/23/little-game-list-wechat-directory-tree/)

<img src="https://raw.githubusercontent.com/lefex/iWeChat/master/image/wechat_catagory.png" title="继承" width="300"/>

**MonkeyDev自动导出头文件**

工程已集成class-dump导出可执行文件OC头文件的功能，可在build settings最下面开启该功能，在 User-Defined 下添加 MONKEYDEV_CLASS_DUMP 值为 YES。

#### 💯第三方库

**基于脚本**

研究某个APP时，需要了解其使用的第三方库，使用 class-dump 导出的头文件非常多，刚靠肉眼查看时，耗时耗力。为了解决这个痛点，便发明了这个工具。下面是获取微信使用的第三方库，可以查看 pod 库的 star 数，源地址。

本工具基于 python 写的，在[这里](https://github.com/lefex/iWeChat/blob/master/python)可以找到源码。下载源码后修改 `file_catagory.py ` 文件的 `IPA_HEADER_PATH` 为 class-dump 导出的头文件目录。执行 `python file_catagory.py `

```
IPA_HEADER_PATH = '/Users/lefex/Desktop/header/xxx'
```

- [pop](https://github.com/facebook/pop.git) - (18872)
- [GPUImage](https://github.com/BradLarson/GPUImage.git) - (17338)
- [WebViewJavascriptBridge](https://github.com/marcuswestin/WebViewJavascriptBridge.git) - (10649)
- [FBSDKCoreKit](https://github.com/facebook/facebook-ios-sdk.git) - (5894)
- [WCDB](https://github.com/Tencent/wcdb) - (5700)
- [GCDWebServer](https://github.com/swisspol/GCDWebServer.git) - (4011)
- [EGOTableViewPullRefresh](https://github.com/enormego/EGOTableViewPullRefresh.git) - (3336)
- [KSCrash](https://github.com/kstenerud/KSCrash.git) - (1942)
- [OpenUDID](https://github.com/ylechelle/OpenUDID.git) - (1909)
- [YYImage](https://github.com/ibireme/YYImage.git) - (1193)
- [SKBounceAnimation](https://github.com/khanlou/SKBounceAnimation.git) - (912)
- [YYAsyncLayer](https://github.com/ibireme/YYAsyncLayer.git) - (405)
- [NSTimer-Blocks](https://github.com/jivadevoe/NSTimer-Blocks.git) - (269)

如果还有没发现的第三方库欢迎提 [issues](https://github.com/lefex/iWeChat/issues)

**通过头文件搜索**

如果APP使用了三方库，可以输入`PodsDummy`来快速找到使用的第三方库和私有库；

<img src="https://raw.githubusercontent.com/lefex/iWeChat/master/image/PodsDummy.png" title="三方库" width="300"/>

#### 💯UI 

除了头文件外，研究第三方 APP 另一个比较重要的点就是查看 UI。可以使用 Reveal 查看视图层级。使用 `MonkeyDev` 可以在非越狱的手机上运行 Reveal。

MonkeyDev 默认集成是最新版本，需要把自己的 `RevealServer.framework`放到`/opt/MonkeyDev/frameworks`下（打开 Reveal，点击 reveal - help - show reveal in finder 即可找到 RevealServer.framework），这样就可以查看时图层级。

如果 Reveal 过期了，直接修改电脑时间为可以继续使用。

![reveal.png](https://upload-images.jianshu.io/upload_images/1664496-77c7d397deb1bea3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



#### 💯继承层级

使用 python 脚本轻松找出继承层级，比如我想找出 `UIWindow` 的继承层级结构，在这里可以找到 [python脚本](https://github.com/lefex/iWeChat/tree/master/python)：

<img src="https://raw.githubusercontent.com/lefex/iWeChat/master/image/iwc_inherit.jpeg" title="继承" width="300"/>

#### 💯数据库设计

数据库的结构是什么，各个表之间是如何关联的，表中保存的数据是什么。

**好友表（Friend）**：每个好友，包含群主，公众号都会保存到这张表中

```
CREATE TABLE Friend (
    userName           TEXT    PRIMARY KEY,
    type               INTEGER DEFAULT 0,
    certificationFlag  INTEGER DEFAULT 0,
    imgStatus          INTEGER DEFAULT 0,
    encodeUserName     TEXT,
    dbContactLocal     BLOB,
    dbContactOther     BLOB,
    dbContactRemark    BLOB,
    dbContactHeadImage BLOB,
    dbContactProfile   BLOB,
    dbContactSocial    BLOB,
    dbContactChatRoom  BLOB,
    dbContactBrand     BLOB
);
```

**消息表（Chat_xxxxxxxxxxxx）**： 每一个会话会生成一张表

````
CREATE TABLE Chat_099cc67071b64517d719cdb9430037d8 (
    TableVer   INTEGER DEFAULT 1,
    MesLocalID INTEGER PRIMARY KEY AUTOINCREMENT,
    MesSvrID   INTEGER DEFAULT 0,
    CreateTime INTEGER DEFAULT 0,
    Message    TEXT,
    Status     INTEGER DEFAULT 0,
    ImgStatus  INTEGER DEFAULT 0,
    Type       INTEGER,
    Des        INTEGER
);
````

**消息撤回表（RevokeMsgTable）**

```
CREATE TABLE RevokeMsgTable (
    MSG_REVOKE_COL_SVRID   INTEGER DEFAULT 0
                                   PRIMARY KEY,
    MSG_REVOKE_COL_CONTENT TEXT,
    MSG_REVOKE_COL_INTRES1 INTEGER DEFAULT 0,
    MSG_REVOKE_COL_INTRES2 INTEGER DEFAULT 0,
    MSG_REVOKE_COL_INTRES3 INTEGER DEFAULT 0,
    MSG_REVOKE_COL_STRRES1 TEXT,
    MSG_REVOKE_COL_STRRES2 TEXT,
    MSG_REVOKE_COL_STRRES3 TEXT
);
```

#### 💯沙盒目录

沙盒目录结构是什么，每个文件夹下面保存了那些数据。

![](https://github.com/lefex/iWeChat/blob/master/image/wc_sandbox.png?raw=true)



#### 💯Pod 集成

如果想使用第三方库咋么办？直接通过 `pod init`，然后在 `Podfile` 里添加你想使用的第三方库即可。

```
target 'xxxDylib' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  # use_frameworks!

  # Pods for KuaiXuoyeDylib
  pod 'xxx'


end
```

#### 💯查看网络请求数据

有时候想快速地查看某个 APP 中的网络请求结果，抓包可能是一个不错的选择，但是遇到HTTPS的请求，就比较费事。其实我们可以通过逆向来查看网络请求，主要有两种方式：

- 找打某个应用中网络请求的统一出口，然后 Hook 掉这个方法，直接拿到数据。不过找到 APP 网络请求封装的类有时候比较难。教你一招，非常容易，找到某个页面中含有网络请求的类，使用 Hopper 工具查看伪代码，非常容易定位具体的网络请求类；
- 使用网络工具直接集成到第三方APP中，通过工具查看网络请求；

## 🐰工具使用说明

#### 💯CaptainHook Hook 代码

```objective-c
// 无参数
CHDeclareClass(WCActionSheet)
CHOptimizedMethod0(self, NSArray *, WCActionSheet, buttonTitleList){
    NSArray *titles = CHSuper0(WCActionSheet, buttonTitleList);
    return titles;
}

CHConstructor{
    CHLoadLateClass(WCActionSheet);
    CHClassHook0(WCActionSheet, buttonTitleList);
}
```

```objective-c
// 一个参数
CHDeclareClass(MMUIImageView);
CHOptimizedMethod1(self, void, MMUIImageView, setImage, NSString *, imageurl){
    NSLog(@"setImage: %@", imageurl);
    CHSuper1(MMUIImageView, setImage, imageurl);
}
CHConstructor{    
    CHLoadLateClass(MMUIImageView);
    CHClassHook1(MMUIImageView, setImage);
}
```

```objective-c
@interface Lefex : NSObject

+ (Lefex *)empty;
- (void)updateNickName:(NSString *)nickName;
- (void)updateNickName:(NSString *)nickName age:(int)age;
- (void)requestNickNameForId:(NSString *)userId completion:(void(^)(NSString *))block;

@end
```

```objective-c
@implementation Lefex

+ (Lefex *)empty {
    NSLog(@"orgin - %@", NSStringFromSelector(_cmd));
    return [Lefex new];
}

- (void)updateNickName:(NSString *)nickName {
    NSLog(@"orgin - %@", NSStringFromSelector(_cmd));
}

- (void)updateNickName:(NSString *)nickName age:(int)age {
    NSLog(@"orgin - %@", NSStringFromSelector(_cmd));
}

- (void)requestNickNameForId:(NSString *)userId completion:(void(^)(NSString *))block {
    NSLog(@"orgin - %@", NSStringFromSelector(_cmd));
    if (block) {
        block(@"lefe_x");
    }
}

@end
```



```objective-c
typedef void(^RequestBlock)(NSString *);

// hook某个类时需要先声明
CHDeclareClass(Lefex)

// Hook 类方法
CHOptimizedClassMethod0(self, Lefex *, Lefex, empty){
    Lefex *me = CHSuper0(Lefex, empty);
    NSLog(@"Hook empty");
    return me;
}

// Hook 一个参数的方法
CHOptimizedMethod1(self, void, Lefex, updateNickName, NSString *, name) {
    CHSuper1(Lefex, updateNickName, name);
    NSLog(@"hook updateNickName");
}

// Hook 两个参数的方法
CHOptimizedMethod2(self, void, Lefex, updateNickName, NSString *, name, age, int, age) {
    CHSuper2(Lefex, updateNickName, name, age, age);
    NSLog(@"hook updateNickName: age");
}

// Hook 带有block的方法
CHOptimizedMethod2(self, void, Lefex, requestNickNameForId, NSString *, userId, completion, RequestBlock, block) {
    RequestBlock nicknameBlock = ^(NSString *nickname) {
        NSLog(@"hook callback :%@", nickname);
        if (block) {
            block(nickname);
        }
    };
    
    CHSuper2(Lefex, requestNickNameForId, userId, completion, nicknameBlock);
    NSLog(@"hook requestNickNameForId: age");
}

// Hook 参数是二级指针的方法
CHOptimizedMethod1(self, void, Lefex, queryLocation, NSString **, name) {
    CHSuper1(Lefex, queryLocation, name);
    NSLog(@"hook queryLocation: %@", *name);
}

CHConstructor {
    // 导入类才能够使用
    // linkable
    CHLoadClass(Lefex);
    // un linkable
//    CHLoadLateClass(Lefex);
    
    CHClassHook0(Lefex, empty);
    CHClassHook1(Lefex, updateNickName);
    CHClassHook2(Lefex, updateNickName, age);
    CHClassHook2(Lefex, requestNickNameForId, completion);
    CHClassHook1(Lefex, queryLocation);
}
```

```verilog
2018-12-12 21:03:13.378534+0800 CaptainDemo[43777:862109] orgin - empty
2018-12-12 21:03:13.378682+0800 CaptainDemo[43777:862109] Hook empty
2018-12-12 21:03:13.378822+0800 CaptainDemo[43777:862109] orgin - updateNickName:
2018-12-12 21:03:13.378919+0800 CaptainDemo[43777:862109] hook updateNickName
2018-12-12 21:03:13.379002+0800 CaptainDemo[43777:862109] orgin - updateNickName:age:
2018-12-12 21:03:13.379097+0800 CaptainDemo[43777:862109] hook updateNickName: age
2018-12-12 21:03:13.379220+0800 CaptainDemo[43777:862109] orgin - requestNickNameForId:completion:
2018-12-12 21:03:13.379299+0800 CaptainDemo[43777:862109] hook callback :lefe_x
2018-12-12 21:03:13.379374+0800 CaptainDemo[43777:862109] orgin callback lefe_x
2018-12-12 21:03:13.379440+0800 CaptainDemo[43777:862109] hook requestNickNameForId: age
2018-12-12 21:03:13.379513+0800 CaptainDemo[43777:862109] orgin - queryLocation:
2018-12-12 21:03:13.379582+0800 CaptainDemo[43777:862109] hook queryLocation: BeiJing
2018-12-12 21:03:13.379670+0800 CaptainDemo[43777:862109] orgin loction: BeiJing
```

#### 💯Logos 语法

http://iphonedevwiki.net/index.php/Logos

```objective-c
// 要 hook 的类
%hook ClassName

// hook 类方法
+ (id)sharedInstance
{
	%log;
	return %orig; // 调用原实现
}

- (void)messageWithNoReturnAndOneArgument:(id)originalArgument
{
	%log;
    // 调用原实现，可以修改参数
	%orig(originalArgument);
}

- (id)messageWithReturnAndNoArguments
{
	%log;

    // 调用原实现，查看返回值，修改返回值
	id originalReturnOfMessage = %orig;
	return originalReturnOfMessage;
}
// 要有结束标签
%end
```

#### 💯查找可执行文件技巧

显示包内容后，按 size 大小排列文件，可直接文件一搬很多；



## 🐼业务逻辑

#### 💯还原某些UI的设计

分析某个 View 是如何设计的并实现它，比如典型的 `ActionSheet`，可以根据头文件来还原它的实现；聊天中的气泡有很多，有非常多的 Cell，那么这种结构是如何设计的呢？

#### 💯探索各个模块业务逻辑

PM 常说，按照微信的加好友逻辑实现就行，擦，你有考虑到微信加好友背后还有哪些你所不知道的逻辑吗？

#### 💯消息类型

[微信消息类型](https://github.com/lefex/iWeChat/blob/master/MESSAGE.md)

#### 💯文件说明


- `iConsoleWindow` 显示的主 Window
- `WAWeb` 为微信小程序类
- `YYWAWebView : WKWebView` 为微信小程序的 WebView



## 🦁错误总结

```verilog
entry point (_main) undefined. for architecture arm64
// 新建文件时，需要把文件建到 xxxDylib 中，不能选择 Target
```

```objective-c
CodeSign /Users/wangsuyan/Library/Developer/Xcode/DerivedData/TVideo-hamzrgdkjpjxzwaloktqyzqrckpm/Build/Products/Debug-iphoneos/libTVideoDylib.dylib
    cd /Users/wangsuyan/Desktop/baidu/reverse/TVideo
    export CODESIGN_ALLOCATE=/Users/wangsuyan/Desktop/Xcode9.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/codesign_allocate
    export PATH="/Users/wangsuyan/Desktop/Xcode9.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/usr/bin:/Users/wangsuyan/Desktop/Xcode9.app/Contents/Developer/usr/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    
Signing Identity:     "iPhone Developer: xx (xxx)"

    /usr/bin/codesign --force --sign CE05AADAA82C40AD173C44316B410B221A24C9AB --entitlements /Users/wangsuyan/Library/Developer/Xcode/DerivedData/TVideo-hamzrgdkjpjxzwaloktqyzqrckpm/Build/Intermediates.noindex/TVideo.build/Debug-iphoneos/TVideoDylib.build/libTVideoDylib.dylib.xcent --timestamp=none /Users/wangsuyan/Library/Developer/Xcode/DerivedData/TVideo-hamzrgdkjpjxzwaloktqyzqrckpm/Build/Products/Debug-iphoneos/libTVideoDylib.dylib

CE05AADAA82C40AD173C44316B410B221A24C9AB: no identity found
Command /usr/bin/codesign failed with exit code 1
// 这个错误是修改了电脑时间
```



## 🙈好文推荐

已经有不少同学对微信有一些探索，把我们认为比较好的文章推荐到这里：

- [**WeChatRedEnvelop 抢红包**  ](https://github.com/buginux/WeChatRedEnvelop)
- [**WeChatPlugin-MacOS Mac微信插件**  ](https://github.com/TKkk-iOSer/WeChatPlugin-MacOS)



## 🐯联系信息

#### 如果想入群，可以先加我的微信好友，备注 iWechat ！！！

<img src="https://raw.githubusercontent.com/lefex/iWeChat/master/image/qrcode.png" title="继承" width="300"/>

## 免责声明

本项目旨在学习微信的设计，不可用于商业和个人其他意图。若使用不当，请使用者自行承担。