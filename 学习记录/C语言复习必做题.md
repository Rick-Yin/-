## 练习0：准备

编辑器选择VSCODE

## 练习1：启用编译器

- 在你的文本编辑器中打开`ex1`文件，随机修改或删除一部分，之后运行它看看发生了什么。
	- 大部分情况下，随机添加或删除会导致编译失败， 显示error并无法生成执行文件。
- 再多打印5行文本或者其它比`"Hello world."`更复杂的东西。
	- 打印了 `“Hello shanghaitech \n in Shanghai \n China \n world \n universal”`
- 执行`man 3 puts`来阅读这个函数和其它函数的文档。

## 练习2：用Make来代替Python

- 改进makefile文件:
	- **添加.PHONY**：使用`.PHONY`来声明`all`和`clean`是伪目标。这样做的目的是防止Make错误地认为这些目标是指向实际文件的，并在文件存在时跳过它们的执行。
	- **改正拼写错误**: 变量`CFLASGG`应为`CFLAGS`。
	- **编译标志**: 添加一个编译指令，使用`$(CC)`变量来表示C编译器。同时，使用`$(CFLAGS)`变量来应用之前定义的编译标志。

...