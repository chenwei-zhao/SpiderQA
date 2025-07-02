# SpiderQA
关于爬虫实践的QA与工具推荐

## Q1: APP抓不到包

- A1: 证书问题，可以ROOT手机，或者使用手机模拟器
- A1: APP设置请求不走代理（如OkHttp发送请求，设置 Proxy.NO_PROXY），可以使用流量转发工具（如Drony）做中转, APP->Drony->Charles/Fiddler

## Q2: WebAssembly 反爬机制

A2: 机制如下图：加密逻辑在wasm中实现，js调用wasm暴露的加密方法

![image](https://github.com/user-attachments/assets/4eedb43d-6378-4a6d-9145-66346919a8e8)


## Q3: Scrapy框架的不足

- A3: 不支持分布式
- A3: 学习曲线陡峭
- A3: 存在Request丢失的情况（spider代码报错或者Request超出重试次数会丢失）

## Q4: 开源验证码识别工具

- A4: [ddddocr](https://github.com/sml2h3/ddddocr "ddddocr")
- A4: [captcha-recognizer](https://github.com/chenwei-zhao/captcha-recognizer "captcha-recognizer")

## Q5: Ocr工具
  
- A5 [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR "PaddleOCR") (文本定位识别)

## Q6: 小程序反编译工具
- A6: [wxapkg](https://github.com/wux1an/wxapkg)
- A6: [e0e1-wx](https://github.com/eeeeeeeeee-code/e0e1-wx)
