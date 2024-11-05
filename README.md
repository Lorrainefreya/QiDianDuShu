# 起点读书 QiDianDuShu
搬运自 https://www.52pojie.cn/thread-1820936-1-1.html (出处: 吾爱破解论坛)

## 起点脚本7.3更新
优化：再次优化解决，因网络波动或其他手机未知卡顿，产生的广告视频未加载成功而直接跳过，并弹出‘广告已经看完了，直接给你奖励吧’文字时，脚本陷入死循环的问题

新增：青少年模式弹窗，流量播放弹窗过滤

Bug阉割：因为抽奖页面的未知改动，现在抽奖功能已经不能用了，抽奖页面所有控件均不能获取到，所以暂时屏蔽该功能，直至我找到新的解决方法

版本前瞻：广告播放页面最近有部分朋友又变回旧版页面了，不过貌似之前的开发代码时做的兼容性预判生效了，所以暂时对该部分功能观察一段时间确认是否稳定，是否存在优化空间
关于版本号的问题，每次更新版本号不连续是因为我在优化代码时淘汰了中间测试版本，每个上线版本都是经过大约3天的稳定性试用才发布的

注：脚本每次更新都是对旧版兼容的，新旧的福利中心或者签到页都是兼容



## 历史版本
起点脚本2.0更新  
经过一段时间的测试，再一次优化了代码，进一步降低点击事件的失效问题。  
另经过最近的测试，平板电脑不能使用该代码，因为楼主是使用图层来定位某些按键的，平板的图层与手机的不同会导致代码点击事件失效一大部分，目前不打算修复这个问题，等哪天闲下来再说吧。  
————————————————————————  
起点脚本3.0更新  
优化+控件的点击，移除通过图层来获取控件的操作，通过坐标计算点击位置，好处是点击的位置更准确，坏处是脚本运行期间如果弹出意外弹窗（微信消息之类的横屏弹窗）会误点导致脚本运行出错。  
运行脚本的手机如果太远古，会因为各种应用卡顿导致脚本运行出问题（例如打开某个页面反应过慢会一直点击，导致最后同一个页面打开很多个），暂不修复这个问题，优化这玩意好难，永远不知道旧手机会卡在哪一步……  
————————————————————————  
起点脚本4.0更新  
新增：兼容两种版本的起点签到页，即，签到获取经验和签到获取章节卡碎片两种版本  
注：周日章节卡碎片兑换的操作还是要自己来，因为我也不知道你要换哪一种章节卡，还是自己按照需求换吧  
————————————————————————  
起点脚本5.1更新  
在原计划发布的5.0版本基础对观看视频的代码逻辑进行了优化，至于未发布的5.0已经被淘汰了，原因是我发现最近起点的看视频时长有增加的趋势，就是说原本绝大部分视频都是看小于等于15秒视频即可获取，但是最近出了一个所谓的“白泽装扮”，视频时长是观看随机的小于等于30秒才可以获取，这是一个信号，意味着后续视频福利的观看时长可能会增长（实际上有一次我在网络波动的情况下测试脚本，开宝箱的视频竟然是观看20秒才可以领取），所以我取消了原计划11月13号发布的脚本5.0，进行延期优化。另外星期二我老爸突然受伤了，我去医院照顾了几天，耽误了点时间今天才写好，而且由于时间匆忙，代码稳定性的测试还没进行就在今天匆匆发布了，大家有问题，多多提出（附截图，以及语言描述，最好是稳定复现的问题，比较好解决）  
新增：兼容新版开宝箱福利中心，优化观看视频代码逻辑。  
————————————————————————  
起点脚本5.2.5更新  
新增：兼容安卓14与鸿蒙，安卓13及以下设备。  
优化：修复新版视频播放页面脚本失效的问题  
————————————————————————  
起点脚本5.2.6更新  
优化：进一步优化5.2.5的稳定性（针对安卓14的优化；鸿蒙，安卓13及以下设备可不更新）  
————————————————————————  
起点脚本5.2.7更新  
优化：针对高频问题2的优化，注意是优化，不是完全杜绝，只是在遇到该问题时，可以跑下去，不至于卡住。  
————————————————————————  
起点脚本5.2.8更新  
新增：高频问题3的识别文字补充。  
————————————————————————  
起点脚本5.2.9更新  
修复：修复安卓14系统，有概率卡在“观看视频0秒后，可领取奖励”界面的问题  
优化：修改获取退出坐标的逻辑，增加稳定性  
————————————————————————  
起点脚本5.2.10更新  
修复：修复鸿蒙，安卓13及以下系统，在“观看完视频”的界面运行异常，自动打开应用跳转的问题  
————————————————————————  
起点脚本6.0更新  
新增：引入模块功能，可以单独启用依附于本脚本的模块脚本，用于添加自定义功能

————————————————————————  

起点脚本6.1更新  
新增：听书一分钟领取起点币功能  

————————————————————————

起点脚本6.1.5更新
新增1：根据反馈，新增听书静音功能，但该功能需要授权“修改系统设置权限”；这里着重为小白强调一下：“修改系统设置权限”是仅次于root权限的，授权该权限几乎相当于授权控制手机所有功能，如果你的auto.js或autox.js来源并不正规，有被内置病毒概率，那么并不建议你授权该权限，请注释掉第10行,11行代码，每次使用前，先手动静音也挺好的，我衷心的不希望在“病毒救援区”与各位碰面。
新增2：增加听书防黑屏功能
优化：起点7.9.336.1206版安卓13及以下系统已经可以稳定获取看视频控件了，所以和安卓14的看视频逻辑进行了合并，稳定性提高，并彻底解决高频问题2，3，以后不需要根据系统类型来区别处理了，所有系统采用一套看视频逻辑。
修复：解决偶尔跳过每日视频观看的bug
预开发：针对新出现的听书广告（评论区置顶），做了预开发，但因为我始终没有遇到过该广告，所以该功能仅在理论上是可以使用的，如果后续有问题，请及时反馈，我来修改。

————————————————————————


起点脚本6.1.6更新
修复1：修复因签到页布局改变导致的抽奖看视频退出异常的问题
修复2：修复因第三方广告跳过软件误触，导致视频暂停播放的问题（例如“李跳跳”，“GKD”在视频广告页面因识别到了“跳过广告”文字而产生误触，造成的视频停止播放）
优化：以后每次更新会将代码文档打包，以附件的形式放在本帖最后，这样没有电脑的小伙伴只需下载附件再解压，最后长按解压后的文档，根据手机的弹窗，选择auto.js或autox.j自带的“导入脚本文件”功能直接使用（便捷是有代价的，需要1吾爱币）

————————————————————————

起点脚本6.1.7更新
修复：解决偶尔获取不到退出坐标脚本卡死的问题

————————————————————————

起点脚本6.1.8更新
修复：修复因听书界面改版导致的听书异常问题（无法听书或听完书退不出去）

————————————————————————

起点脚本6.1.9更新
修复：修复因听书界面改版导致的听书异常问题（无法听书或听完书退不出去）；这次更新就是在回退至6.1.7版本的基础上添加了一点容错机制，一定程度上避免再次出现界面改版导致的问题，理论上直接使用6.1.7版本也是可以的。

————————————————————————

起点脚本6.1.9.1更新
修复：解决异常退出福利中心的问题

————————————————————————

起点脚本6.1.10.2更新
修复：解决因网络波动或其他手机未知卡顿，产生的广告视频未加载成功而直接跳过，并弹出‘广告已经看完了，直接给你奖励吧’文字时，脚本陷入死循环的问题


