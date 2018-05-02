# Sunwaypay API 文档


## 1.文档说明

> 该文档为`sunwaypay`商户对接文档,本文档会根据后期接口升级一同升级

* 商户管理后台网址：[https://merchant.sunwaypay.org](https://merchant.sunwaypay.org)
* 神威支付前台网址：[https://www.sunwaypay.org](https://www.sunwaypay.org)
* API文档同步网址：[https://sunwaypay.gitbook.io/sunwaypay-api-doc/](https://sunwaypay.gitbook.io/sunwaypay-api-doc/)

## 1.1.版本说明

+ 该文档为第1版本，版本号`v1.0`，下一版从次版本号开始

## 1.2.签名规则

+ 签名规则采用md5\(请求参数+商户密钥\)进行组装,详实请阅读请求参数部分

## 1.3.验签规则

+ 验签规则，将`POST`接收参数+商户自己的密钥按照指定的顺序进行拼接后`md5`加密，然后和接收数据中的签名  
+ 进行对比，对比成功表示数据未被篡改，此时可以执行自己的业务逻辑
