我们在使用Word编辑文档，或者使用Excel表格计算时，时常想，要是有个版本管理工具能把我们的文档或表格管理起来就好了，好让我们可以“昨日重现”，或在任意版本间穿梭！

git就是一个使用便捷，功能强大的工具，在编程界可谓鼎鼎大名，可以说是程序员的必备工具。但是，git只能对代码等文本文件进行版本管理，对Microsoft的Word、Excel等二进制文档却无能为力。

base64命令可以把二进制文件编码成可打印文本文档，当然，也可以解码成二进制文档。何不把它git工具结合起来使用呢。

Word/Excel文件编辑完成后，将其base64编码，然后使用git提交；需要某个版本时，再通过git reset命令将其取回，然后，使用base64 --decode解码成二进制文件。

现在的想法是，把这这两个工具集成起来，做一个增强版的Git GUI，就叫BinaryGit吧，便于普通户使用。
