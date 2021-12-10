### ProxyScan

自动化扫描SQL注入

### 开发原因：

因为之前得ProxySqlmap很多人反映会把自己IP封掉，所以就改成自己加入Payload了

### 使用方式：

#### 设置端口：

![image](https://user-images.githubusercontent.com/36424999/144794420-a4e0ef47-40d4-4bf3-9769-5fd09d3ee748.png)

在配置->代理设置中设置端口，软件会自动监听此端口，默认监听8081：

![image](https://user-images.githubusercontent.com/36424999/144794485-b8405743-36b6-4d9c-92d5-ae6aa903e42b.png)

#### 设置域名：

域名使用正则表达式进行设置，如你需要测试百度(.*).baidu.com

![image](https://user-images.githubusercontent.com/36424999/144794654-fde8172f-fa47-49ba-99be-b0f42297527f.png)

#### 信息泄露：

软件加入了信息泄露检测得功能，依然是使用正则表达式，会自动匹配返回页面。

![561954ffe774f63772b5a5ec179b9027](https://user-images.githubusercontent.com/36424999/144794798-c1373c36-85d2-477f-ba5e-9877d6d07b12.png)

#### 使用方式：

在设置中点击开启就能使用了，**将浏览器代理设置为127.0.0.1:8081**，注意是浏览器代理不是系统代理。

![0e3bf6138c231b4ca66c299f6c1398d](https://user-images.githubusercontent.com/36424999/144794971-2f5c426b-ab1b-4463-93ac-e5bfdd6c6380.jpg)

### 联系方式：

**对于提供宝贵意见的用户将会参与到下个版本的测试中，预计会加入自动测试常见设备弱口令、XSS、SSRF的扫描。**

微信:xuanyuwd，备注：建议意见

### 更新日志：

```
2021-12-10 更新Log4j RCE检测
```
