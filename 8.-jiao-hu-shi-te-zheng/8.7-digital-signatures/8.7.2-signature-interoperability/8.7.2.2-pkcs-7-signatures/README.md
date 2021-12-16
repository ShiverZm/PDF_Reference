# 8.7.2.2 PKCS#7 Signatures

当使用PKCS#7签名时，Contents的值是DER编码 包含签名的二进制数据对象。

SubFilter可以采用下列值之一:

* **adbe.pkcs7.detached:**在PKCS#7 signed-data字段中没有封装任何数据
* **adbe.pkcs7.sha1:**字节范围的SHA1摘要封装在 PKCS#7带数据类型的ContentInfo的signed-data字段。

PKCS#7对象必须符合Internet RFC中的PKCS#7规范,PKCS #7:加密消息语法，版本1.5(参见参考书目)。至少，它必须包含签名者的X.509签名证书。该证书用于验证“Content”中的签名值。

PKCS#7对象可以有选择地包含以下属性:

* 时间戳信息作为无符号属性(PDF 1.6):时间戳标记必须符合RFC 3161，必须计算并嵌入到在RFC 3161的附录A中描述的PKCS#7对象。
* 作为签名属性的撤销信息(PDF 1.6):该属性可以在中包含执行撤销所需的所有撤销信息检查签署者的证书及其颁发者的证书。
* 来自签名者信任链的一个或多个颁发者证书(PDF 1.6);•一个或多个与签署人证书cate相关的RFC 3281属性证书(PDF 1.7)。
