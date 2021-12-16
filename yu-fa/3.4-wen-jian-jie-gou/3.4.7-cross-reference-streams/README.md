# 3.4.7 交叉引用流

从PDF 1.5开始，交叉引用信息可以存储在交叉引用流中，而不是存储在交叉引用表中。交叉引用流有以下优点:

* 一种更紧凑的交叉引用信息表示
* 能够访问存储在对象流中的压缩对象(见3.4.6节“对象流”)，并允许将来添加新的交叉引用条目类型。

交叉引用流是流对象（请参见第3.2.7节，“流对象”），其中包含字典和数据流。每个交叉参考流都包含对应于交叉参考表（见3.4.3节“交叉参考表”）和预告片（见3.4.4节“文件预告片”）的信息。预告片字典条目存储在流字典中，交叉引用表条目存储为流数据，如下示例所示：

**Example 3.10**

```
... objects ...
12 0 obj           % Cross-reference stream
    << /Type /XRef % Cross-reference stream dictionary
    /Size ...
    /Root ...
>>
stream
... % Stream data containing cross-reference information
endstream
endobj
... more objects ...
startxref 
byte_offset_of_cross-reference_stream % Points to object 12
%%EOF
```

请注意，startxref关键字后面的值现在是交叉引用流的偏移量，而不是xref关键字。(请参见附录H.中的实现说明21)对于完全使用交叉引用流的文件（即参见PDF1.5）请参见第109页上的“与不支持PDF1.5的应用程序的兼容性”)，关键词xref 和 trailer不再使用。因此，除了startxref地址%%EOF段和注释外，PDF1.5文件完全是一个对象序列。注：在线性化的PDF中允许使用对象流和交叉引用流，并对规范进行少量修改（参见F.2节，“线性化的PDF文档结构”）。
