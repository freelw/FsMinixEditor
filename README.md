## FsMinixEditor

FsMinixEditor 是一个可以解析和制作minix1.0文件系统镜像的工具，使用nodejs编写。


###使用

* 首先需要安装依赖


	npm install


* 使用时有两种模式
	
	1.解析模式 将一个文件系统解压到一个目录
	
	```
	node minix_fs_editor.js -i img/simple.img -d release
	```
	2.压缩模式 将一个目录作为根目录制作文件系统镜像
	
	```
	node minix_fs_editor.js -d release -o out.img
	```
	这里将out.img挂在到linux0.12的软驱上是可以被识别的