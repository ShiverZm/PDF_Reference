# 8.5.3 动作类型

PDF支持表8.48中列出的标准动作类型。下面的部分详细描述了每种类型。扩展的插件可以添加新的动作类型。

表8.48

| Action Type  | Description                                | Discussed in Section |
| ------------ | ------------------------------------------ | -------------------- |
| GoTo         | 在当前文档跳转到目的地                                |                      |
| GoToR        | （“Go To Remote”）在另一个文档跳转到目的地               |                      |
| GoToE        | ("Go to Embedded";PDF1.6)在嵌入的文档中跳转到目的地     |                      |
| Lauch        | 启动一个应用程序，通常是打开一个文件                         |                      |
| Thread       | 开始阅读文章                                     |                      |
| URI          | 解析统一资源标识符（Uniform Resource Identity）       |                      |
| Sound        | (PDF1.2) 播放音乐                              |                      |
| Movie        | (PDF1.2) 播放电影                              |                      |
| Hide         | (PDF1.2) 设置注释隐藏标志                          |                      |
| Named        | (PDF1.2) 通过查看器应用执行某个动作的提前定义                |                      |
| SubmitForm   | (PDF1.2)提交数据到URL(Uniform Resource Locator) |                      |
| ResetForm    | (PDF1.2)设置项的默认值                            |                      |
| ImportedData | (PDF1.2)从文件中导入字段值                          |                      |
| JavaScript   | (PDF1.3)执行一个JavaScript脚本                   |                      |
| SetOCGState  | (PDF1.5)设置可选内容组的状态                         |                      |
| Rendition    | (PDF1.5)控制多媒体内容的播放                         |                      |
| Trans        | (PDF1.5)使用转换字典更新文档的显示。                     |                      |
| GoTo3DView   | (PDF1.6)设置3D注释的当前视图                        |                      |

注意:以前版本的PDF规范描述了一个动作类型称为set-state动作;这种类型的动作，现在被认为是过时的，它的用途是不再推荐。在附加动作类型中，定义了另一种操作类型，即无操作动作（PDF 1.2），但从未实现;它不再被定义，应该被忽略。
