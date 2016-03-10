# mazeGame   迷宫游戏完整版
maze.html与maze仓库中的一样，maze2.html添加了选择难度功能，mazeIntact.html是完整版游戏，下面主要介绍mazeIntact.html文件
游戏功能：提供不同级别的游戏 具体难度迷宫可由maze.html来绘制
          计时功能
          token边界限制
          游戏出口和入口
          排名榜
  为了游戏效果，采用了bootstrap，按钮样式，以及模态框来实现排名榜
  该游戏用localStorage来实现存储功能，也可以用AJAX来实现，将墙信息存到json里就可以
(1)<input type='radio' name='level'>单选框，要求不同input标签的name值相同
(2)计时功能通过定时器实现
(3)排名榜应用数组函数
      
arr.sort();实现按字符串排序
按数值排序，则要写比较函数作为sort的参数
function compare(a,b){
  return a-b;// 从小到大的顺序
  return b-a;//从大到小的顺序
}

js实现模态框调用
```javascript
$("#myModal").modal('shohw');
```
(4)文本垂直居中（仅适用于单行文本和图片）
```javascript
div{
height:80px;
line-height:80px;//设置行高和父元素文本高度相同
}
  <div>垂直居中</div>
```
对于vertical-align仅适用于有valign属性的元素，th,td,caption(表格标题)
或者行内元素在行内元素中的位置：
```javascript
<p><img style='vertical-align:middle/top/bottom....></p>
```
(5)$().append(),$().after(),$().remove()

**其他的已经在maze.html中写过了，就不在这里重复了**
