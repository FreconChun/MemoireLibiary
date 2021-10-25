#  工程记录

每天都来，记录工程

## **2021.10.09**
    【Cloud Database】优化了Cloud中存储的资源数据结构，但是本地没有相应的修改
    【Flags】启动了一个提醒小工具

## **2021.10.08**
    【MAsset】一个全新的用来处理云端资料的组件，目前调试了全部拉去云端资料
    【CloudKit】除了otis和jessica其他都已经做到云端

## **2021.10.07**  【🚩commit】
    【MUser】接入了swift error handling，用来处理异步访问数据库时的问题
    【MUser】优化了异步代码
    【MimageEditor】加入了历史记录跟踪的功能，并且完成了图片的传值
    【ImageCropperView】调整了拖拽手势的函数算法，之前和Rotate结合会出现不跟手的问题（之前运动时没有考虑rotate）
    【UserManager】调试完成了MImage的上下载功能

## **2021.10.06**
    【MColor&DesignSystem】设计了颜色关系，并且根据颜色设计规范重新调整了颜色值

## **2021.10.03**
    【MImage】测试了iconview的样式，但是发现写在Package里面很容易报BAD ACCESS的错误，不知道是渲染逻辑和数据处理起了冲突（因为数据从Data开始加载的），还是因为package中加入frame、resiable之类的函数出了问题（我更倾向于前者），看来之后有必要系统学习concurrnecy。为了实现功能，目前将渲染的函数放在了应用主体内


## **2021.10.02**
    【MImage】支持了相册和拍照添加照片（目前仅可以编辑，不能添加，不能覆盖选择）
    【NOTE】UIImage里有一种隐含的方向，会影响我的裁切函数，因此一开始利用CGImage把所有的图片统一方向之后在裁切
            裁切时也考虑了方向
    【Location，MImageEditor】修改了代码结构从而优化横屏体验

## **2021.10.01**
    【Memoire】从Allinlist中迁移并且重写了MImage的编辑器，目前除了相册和拍照之外其他都可以了
            ⚠️需要统一一下MImage以icon形式渲染的样式
    【CustomizeOverlay】popup 的滑动取消变成可选功能（目前还未做好），现在是锁定只能通过按钮取消
    【Memoire】优化了NavigationView(UserInfoEditview)的结构，从而实现Map的全屏效果

## **2021.09.30**
    【Memoire】 登陆功能完善，对于图片的完全支持
    【MImage】重写逻辑，从数据中读取，支持cloudkit
    【CustomizeOverlay】popup出了一些问题，对于NavigationView配合使用会让控件无响应
            用translucent background的 fullscreen cover解决了这个问题，感谢stackoverflow
    【LocationManager】引入了AllinList中对于地理位置的处理工具，运行状态良好

## **2021.09.29**
    【Memoire】cloudkit + sign in with apple 制作了UserManager,UserInfoEditView,LogInView
    ⚠️**【BUG】登陆之后应该先进入编辑个人信息页面（大概吧），目前无法唤起该页面**
    ⚠️**【TODO】将MImage根据Cloudkit的需求进行更新,目前无法与Cloudkit上传用户头像**

## **2021.09.28**
    【UIComponents】将Symbol改为MImage并且完善文档和内容
    【UIComponents】新建了roataion控制的相关修饰符，并且将原本基于GeometryReader的RStack改名问GStack，新增加基于Rotation的RStack
    【Memoire】设计完成MemoireCard

## **2021.09.26**
    【MemoireLibrary】创建了新的用于记录各种文档的Package

## **2021.09.25**
    【UIComponents】三天时间用Blender完成logo制作

## **2021.09.22**
    【UIComponents】完成了MColor颜色设计规范
    【UIComponents】优化了UIComponents的部分文档和文档结构
    【UIComponents】向Symbol中提供了默认的图片 （stickers 和 usericon）

## **2021.09.21**
    *昨天好像忘写记录了，不过好在没写啥内容,今天补一下*
    【UIComponents】完成一套字体控制系统 MFont
    【UIComponents】更新主文档（UIComponents）

## **2021.09.19**
    【UIComponents】完成RStack并将其实现方法转换成Geometry
    【UIComponents】完成了Device类设备类型检测和设备方向检测

## **2021.09.18**
    【UIComponents】制作一个RStack 目前有些失败

## **2021.09.08**
    【UIComponents】The nil-coalescing operator (??) 支持Binding

## **2021.09.07**
    【UIComponents】CustomizeOverlay模块的编写、代码复查、文档编撰
    【UIComponents】整理了文档结构

## **2021·09·06** 【🚩commit】
    【UIComponents】完成了Alert相关搭建

