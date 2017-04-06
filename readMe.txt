函数注释：
createElements()：生成解锁面板所需要的相应元素，组件由id=‘mydiv’的div包裹，默认添加到body节点内部。
settings()：设置元素宽高，位置。将svg的viewbox与视口对齐。
createLine()：指定命名空间创建SVG折线元素。
createText()：将相应内容显示在页面上持续一段时间。
bindEvens():
   1.为svg里的circle绑定touchstart事件
	2.若触发touchstart事件，记录第一个点，并同时绑定touchmove和touchend。
2.1 touchmove：由于该事件e.target无法实时监听，所以使用document.elementFromPoint(X, Y)来进行事件委托。
2.2 touchend：主要进行密码检测和文字提示。密码存于localStorage.realcode变量。



