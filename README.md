# koa2-fileupload  前端图片压缩上传
在移动端压缩图片并且上传主要用到filereader、canvas 以及 formdata 这三个h5的api。逻辑并不难。整个过程就是：  
　　（1）用户使用input file上传图片的时候，用filereader读取用户上传的图片数据（base64格式）  
　　（2）把图片数据传入img对象，然后将img绘制到canvas上，再调用canvas.toDataURL对图片进行压缩  
　　（3）获取到压缩后的base64格式图片数据，转成二进制塞入formdata，再通过XmlHttpRequest提交formdata。  
如此三步，就完成了图片的压缩和上传。

详情，见[链接](http://www.cnblogs.com/shinefon-2-2/p/5901330.html)   
[参考](http://wangyong31893189.iteye.com/blog/1695472)
[参考移动端图片上传旋转、压缩的解决方案 ](https://github.com/lin-xin/blog/issues/18)
