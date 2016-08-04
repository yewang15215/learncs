# 测试

## 单元测试
* [大牛们都是怎么进行UnitTest 的？](https://www.zhihu.com/question/27313846)


## TDD (Test Driven Development)
* [unicodeveloper/awesome-tdd](https://github.com/unicodeveloper/awesome-tdd) Curated list of awesome resources: books, videos, articles about using TDD

## Test Automation 自动化测试
### 工具
* [macaca]()
* [karma]()

## Testing Framework 测试框架
* Node.js
    - [mocha](https://github.com/mochajs/mocha)

## Penetration Testing 渗透测试
* [enaqx/awesome-pentest](https://github.com/enaqx/awesome-pentest)

## 平台
* Android
    - [hotchemi/awesome-android-testing](https://github.com/hotchemi/awesome-android-testing) A curated list of awesome android testing libraries.
    - [TestFairy](http://www.testfairy.com/)  Android & iOS Mobile Beta Testing


* 游戏测试
    - [K9test](http://www.k9test.com/)

## 持续集成 CI  Continuous Integration
* [Jenkins]()
* [Travis CI](https://github.com/travis-ci/travis-ci)  
* [GitLab](https://about.gitlab.com)
* [Strider](https://github.com/Strider-CD/strider)
* [janky](https://github.com/github/janky)
* [buildbot](https://github.com/buildbot/buildbot)


## 测试工具
* Instrumentation
    - 是早期Google提供的Android自动化测试工具类，虽然在那时候JUnit也可以对Android进行测试，但是Instrumentation允许你对应用程序做更为复杂的测试，甚至是框架层面的。通过Instrumentation你可以模拟按键按下、抬起、屏幕点击、滚动等事件。Instrumentation是通过将主程序和测试程序运行在同一个进程来实现这些功能，你可以把Instrumentation看成一个类似Activity或者Service并且不带界面的组件，在程序运行期间监控你的主程序。缺点是对测试人员来说编写代码能力要求较高，需要对Android相关知识有一定了解，还需要配置AndroidManifest.xml文件，不能跨多个App。
* Monkeyrunner
    - 是Android SDK提供的测试工具。严格意义上来说MonkeyRunner其实是一个Api工具包，比Monkey强大，可以编写测试脚本来自定义数据、事件。缺点是脚本用Python来写，对测试人员来说要求较高，有比较大的学习成本。
* Robotium
    - 是基于Instrumentation的测试框架，目前国内外用的比较多，资料比较多，社区也比较活跃。缺点是对测试人员来说要有一定的Java基础，了解Android基本组件，不能跨App。
* UIAutomation
    - 是Android提供的自动化测试框架，基本上支持所有的Android事件操作，对比Instrumentation它不需要测试人员了解代码实现细节（可以用UiAutomatorviewer抓去App页面上的控件属性而不看源码）。基于Java，测试代码结构简单、编写容易、学习成本，一次编译，所有设备或模拟器都能运行测试，能跨App（比如：很多App有选择相册、打开相机拍照，这就是跨App测试）。缺点是只支持SDK 16（Android 4.1）及以上，不支持Hybird App、WebApp。
* Espresso
    - 是Google的开源自动化测试框架。相对于Robotium和UIAutomator，它的特点是规模更小、更简洁，API更加精确，编写测试代码简单，容易快速上手。因为是基于Instrumentation的，所以不能跨App。