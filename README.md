# LayaBox官网

#### 项目介绍

[演示地址](https://struggle-wjf.gitee.io/layabox_official_website)

- LayaBox官网基于bootstrap响应式布局
  
- 设配到320px;
  
- 项目最大特点：大多数使用珊栏格布局，方便快捷。
  
> 有一些比较大的图片会在固定的设配下隐藏

| 尺寸 | 超小屏幕手机 (<768px) |  小屏幕平板 (≥768px)|中等屏幕桌面 (≥992px)|大屏幕桌面 (≥1200px)|
| :-------------------------:   | :----------: | :----------:  |:----------:  |:----------:  |
|.visible-xs-*|	可见	|隐藏	|隐藏	|隐藏|
|.visible-sm-*	|隐藏	|可见	|隐藏	|隐藏|
|.visible-md-*	|隐藏	|隐藏	|可见	|隐藏|
|.visible-lg-*	|隐藏	|隐藏	|隐藏	|可见|
|.hidden-xs	|隐藏	|可见|	可见	|可见|
|.hidden-sm	|可见	|隐藏	|可见	|可见|
|.hidden-md	|可见	|可见	|隐藏	|可见|
|.hidden-lg	|可见	|可见	|可见	|隐藏|

> 重点是媒体查询

- 媒体查询
  
在栅格系统中，我们在 Less 文件中使用以下媒体查询（media query）来创建关键的分界点阈值。

```css
/* 超小屏幕（手机，小于 768px） */
/* 没有任何媒体查询相关的代码，因为这在 Bootstrap 中是默认的（还记得 Bootstrap 是移动设备优先的吗？） */

/* 小屏幕（平板，大于等于 768px） */
@media (min-width: @screen-sm-min) { ... }

/* 中等屏幕（桌面显示器，大于等于 992px） */
@media (min-width: @screen-md-min) { ... }

/* 大屏幕（大桌面显示器，大于等于 1200px） */
@media (min-width: @screen-lg-min) { ... }
我们偶尔也会在媒体查询代码中包含 max-width 从而将 CSS 的影响限制在更小范围的屏幕大小之内。

@media (max-width: @screen-xs-max) { ... }
@media (min-width: @screen-sm-min) and (max-width: @screen-sm-max) { ... }
@media (min-width: @screen-md-min) and (max-width: @screen-md-max) { ... }
@media (min-width: @screen-lg-min) { ... }

```
