基于 TcpClient 现实的 http请求库，编写于2007年做了几年数据采集工作。

# 支持支持

* http(不支持https)
* get/post
* gzip/deflate 自动解压内容
* 普通响应/chunk响应
* cookie 管理(兼容性好)

# 使用方法

```csharp
TcpClientHttpRequest hr = new TcpClientHttpRequest();
hr.Action = "http://www.baidu.com/";
hr.Method = "get"; //默认
hr.Send();
Console.WriteLine(hr.Response.Xml);
```
