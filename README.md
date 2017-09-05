# -webAPP-
# **1** meta
	
	<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
	
在head头标签中加入该meta,会让页面的宽度强制与设备视图宽度相同，
并且设置了initial-scale(初始化缩放比例)，maximum-scale(最大的缩放比例), 以及设置了user-scalable来禁止用户进行缩放操作。

注意

```
To improve accessibility on websites in Safari, users can now pinch-to-zoom 
even when a website sets user-scalable=no in the viewport.
```

这段翻译过来就是: **为了提高Safari中网站的辅助功能，即使网站在视口中设置了user-scalable = no，用户也可以手动缩放。**

# **2** 获取滚动条的值

在PC端浏览器中获取滚动条的值可以用window.scrollLeft和window.scrollTop来获取， 安卓移动设备也可以通过该属性来获取， 但是在苹果设备中却不会获取到滚动条的值，该值为undefined,只能通过window.scrollX和window.scrollY来进行获取

	window.scrollX 获取横向滚动条滚动距离
	window.scrollY 获取垂直滚动条滚动距离
