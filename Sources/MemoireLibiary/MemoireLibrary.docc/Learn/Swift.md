
#  **Learing Note About Swift**


## ** enum like syntax

Extending static member lookup in generic contexts
SE-0299 allows Swift to perform static member lookup for members of protocols in generic functions, which sounds obscure but actually fixes a small but important legibility problem that hit SwiftUI particularly hard.

At this time SwiftUI hasn’t been updated to support this change, but if everything goes to plan we can stop writing this:

    Toggle("Example", isOn: .constant(true))
        .toggleStyle(.switch)


## ** 注释 与 quickhelp
https://developer.apple.com/library/archive/documentation/Xcode/Reference/xcode_markup_formatting_ref/Todo.html#//apple_ref/doc/uid/TP40016497-CH47-SW1
https://juejin.cn/post/6917520941933625358

## ** Docc 的文档语法
https://developer.apple.com/documentation/xcode/formatting-your-documentation-content
注意：framewrok中未暴露的接口不会被制作到文档中

## ** Timer **
https://www.hackingwithswift.com/articles/117/the-ultimate-guide-to-timer


## **Swift作用域**
参考网站： https://blog.csdn.net/liuyinghui523/article/details/108983314
说明： 通常情况下使用**internal** 访问级别所修饰的属性或方法在源代码所在的**整个模块都可以访问**。
    如果是框架或者库代码，则在整个框架内部都可以访问，**框架由外部代码所引用时，则不可以访问**。
    如果是 App 代码，也是在整个 App 代码，也是在整个 App 内部可以访问。
    **5种修饰符访问权限排序  open > public > interal > fileprivate > private**

## **@inlinable**
参考网站：https://www.jianshu.com/p/d60c0e163944

## **tuple to array**
```swift
    public static var userIconsArray: Array<(label:String,value: MImage)>{
        Array(Mirror(reflecting: userIcons).children) as! Array<(label:String,value: MImage)>
    }
```

## ** NSPredicate
https://www.cnblogs.com/motoyang/p/4858625.html

## ** CloudKit
https://www.hackingwithswift.com/read/33/6/reading-from-icloud-with-cloudkit-ckqueryoperation-and-nspredicate

## ** Combine
https://zhuanlan.zhihu.com/p/154621268

![combine 课本]https://heckj.github.io/swiftui-notes/
