#  Learning SwiftUI

## **PREVIEW**
- framework的预览需要将target切换到对应的framework

## **SwfitUI + Sign In With Apple + Cloud Kit
https://levelup.gitconnected.com/swiftui2-integrate-sign-in-with-apple-to-cloudkit-2020-265506e202e4

DispatchQueue.main.async 保证状态在主线程刷新

##  NavigationView  NavigationLink的背景
NavigationView的背景可以是整个的背景，ignoresafearea后可以填充
NavigarionView内容物的背景是NavigationView的背景，现在可以整个把颜色换了
navigationLink的Background在navigationtitle之后，视图最外面用就可以生效


## Transition
当transition退出不起作用，可能是需要显示提供zindex 保证离开时的视图层级不变
也有可能需要在视图变化处显式使用withAnimation

## sheet
一次只会显示一个sheet 第二个sheet将会在第一个sheet消失后显示

##Text yyds

## Material
material之后使用.cornerRadius再使用shadow就不会继承到所有子视图

## Focused 请配合 task 使用 而不是 onappear
