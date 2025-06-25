# SpiderQA
关于爬虫实践的QA与工具推荐

## Q1: APP抓不到包
- A1: 证书问题：ROOT手机，或者使用手机模拟器
- A2: APP设置请求不走代理（如OkHttp发送请求，设置 Proxy.NO_PROXY）：使用流量转发工具（如Drony）做中转, APP->Drony->Charles/Fiddler
