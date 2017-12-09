#blog
最近在看《图解HTTP》，如题，这个正好与http请求有关，也是面试中及其常见的题目
1. 输入`url`后，客户端向服务端发起请求，浏览器解析`url`里的域名，并进行
`DNS`解析出对应`ip`，路由查找这个地址
2. 找到`ip`后，`tcp/ip`建立连接，客户端发送请求的过程是在报文首部增加信息，服务端接收请求的过程是将报文首部增加的信息去掉
3. 服务端收到请求后会将资源发送给客户端，此时客户端会去接收响应，浏览器对内容进行解析
4. 若浏览器接收到的是`html`页面，解析过程：
    ![image](http://upload-images.jianshu.io/upload_images/5980872-e9679ff90a79b1a0?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
    - 构建`dom`树
    - 构建`css om`
    - 整合`dom`和`css om`，构建`render`树
    - 布局`render`树
    - 绘制`render`树

注：有不足之处后续补足
