# QphotoRenamer

QphotoRenamer 是一个用于批量重命名照片文件的工具，支持多种图片格式，包括常见的RAW格式。该工具使用Python编写，并使用Tkinter构建用户界面。

## 功能特性

- 支持拖放添加照片文件。
- 批量重命名照片文件。
- 支持查看和显示EXIF信息。
- 支持撤销重命名操作。
- 支持设置重命名样式和语言。
- 支持自动滚动和清空文件列表。

## 安装

### 依赖项

在运行QphotoRenamer之前，请确保已安装以下依赖项：

- Python 3.6+
- exifread
- piexif
- pillow_heif
- ttkbootstrap
- tkinterdnd2

你可以使用以下命令安装这些依赖项：

```bash
pip install exifread piexif pillow_heif ttkbootstrap tkinterdnd2
pip install nuitka

nuitka打包命令：
nuitka --standalone --onefile --windows-console-mode=disable --enable-plugin=tk-inter --include-package=exifread --include-package=piexif --include-package=pillow_heif --include-package=ttkbootstrap --include-package=tkinterdnd2 --include-data-file=QPhotoRenamer.ini=QPhotoRenamer.ini --include-data-file=logo.ico=logo.ico --windows-icon-from-ico=logo.ico QPhotoRenamer.py