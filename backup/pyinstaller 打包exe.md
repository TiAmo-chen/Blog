> pyinstaller flappy_bird.py
非单文件
**********
> pyinstaller flappy_bird.py --clean
清理生成的文件
*********
> pyinstaller -F -w flappy_bird.py
-F, --onefile：创建单文件捆绑的可执行文件。
************

**结果待确认**
> pyinstaller -F -w --add-data "resources/*;./resources" flappy_bird.py
这里的--add-data选项告诉PyInstaller将resources文件夹中的所有文件添加到生成的可执行文件中，并在程序运行时将它们放置在./resources目录下。
**********

> pyinstaller -F -w --add-data "resources/*;./resources" flappy_bird.py --upx-dir "D:\LIB\upx-4.2.4-win64"
使用upx压缩生成的文件大小
**************
