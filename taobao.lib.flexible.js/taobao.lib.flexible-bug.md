# ml -- 收集前端实战中的bug
 
## **一、taobao.lib.flexible.js 关于淘宝flexible.js漏洞修补(rem)**  
   
#### 问题： 假设一个网页页面宽度为10rem,设置一个水平居中的图片宽度为 9.2266667rem,在某些机型下，图片横向撑满页面，导致页面布局有误，如下图
 ![image](/taobao.lib.flexible.js/images/2-2三星浏览器页面正常.png)
 
 * 在实战开发中，使用的测试机（ 三星 galaxy s5 型号 sm-g9006v 安卓版本6.0.1 ），在市场上算也算较新的机型
 - rem是根据html的最终font-size进行响应：1rem === finalDocElementFontSize（重点！） 