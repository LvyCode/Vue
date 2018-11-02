# HTML-CSS
```
水平方向 x+y = 100 成立
垂直方向 x+y = 100    
                      20   80    80
                      30   70    70
                      10   90    90
外边距合并出发的条件
  <1>兄弟元素在竖直方向有margin时触发
  <2>父子级元素在竖直方向有margin时触发
解决外边距合并的方案
  <1>外边距起点不同 padding打断
  <2>生成BFC overflow:hidden
        

1.取消行内元素的间隙
	    body{
			font-size: 0;
		} 
2.在行内元素、行内块元素之间是有间隙的
3.块元素独占一行不存在间隙
4.cursor 鼠标样式
  cursor: pointer;小手掌
  cursor: move;鼠标样式
  cursor: wait;标识正在加载
  cursor: help;标识需要帮助
  cursor: url(a.jpg),pointer;自定义鼠标样式，pointer为备用鼠标样式
```