# 8.4.5 注释类型 (Annotation Types)

PDF支持表8.20中列出的标准注释类型。下面各节详细描述每种类型。插件扩展可能会添加新的注释类型，将来还可能添加更多的标准类型。(见附录H实施说明88)

表8.20第一列中的值表示注释字典的Subtype条目的值。第三列表示注释是否为标记注释，如下面的“Markup Annotations”所述。本节还提供了关于不同注释类型的Contents条目值的更多信息。

**表8.20 注释类型**

| ANNOTATION     | TYPE     | MarkUp? 是否有弹窗  | DESCRIPTION |
| -------------- | -------- | -------------- | ----------- |
| Text           | 文本注释     | Yes            |             |
| Link           | 链接注释     | No             |             |
| FreeText       | 开放文本注释   | Yes            |             |
| Line           | 行注释      | Yes            |             |
| Square         | 正方形注释    | Yes            |             |
| Circle         | 圆注释      | Yes            |             |
| Polygon        | 多边形注释    | Yes            |             |
| PolyLine       | 折线注释     | Yes            |             |
| Highlight      | 高亮注释     | Yes            |             |
| Underline      | 强调注释     | Yes            |             |
| Squiggly       | 弯曲强调注释   | Yes            |             |
| StrikeOut      | 删除线注释    | Yes            |             |
| Stamp          | 橡皮图章注释   | Yes            |             |
| Caret          | 插入符号注释   | Yes            |             |
| Ink            | 墨迹注释     | Yes            |             |
| Popup          | 弹出注释     | No             |             |
| FileAttachment | 文件附件注释   | Yes            |             |
| Sound          | 声音注释     | Yes            |             |
| Movie          | 视频注释     | No             |             |
| Widget         | 插件注释     | No             |             |
| Screen         | 屏幕注释     | No             |             |
| PrinterMark    | 打印机的标志注释 | No             |             |
| TrapNet        | 网络限制注释   | No             |             |
| Watermark      | 水印注释     | No             |             |
| 3D             | 3D 注释    | No             |             |

## 注释分类

### 文本注释（便签注释，可打开关闭）

### 自由文本注释（总是显示的 无打开关闭）

### 文本标记注释

* **高亮显示**
* **下划线显示**
* **删除线**
* **锯齿状**
* **下划线显示**
