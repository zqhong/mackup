# Mackup

配置文件备份工具

## 改动

取消链接备份的方式，改为复制备份。

好处：备份/恢复过程中，不会对源文件造成影响。<br>
坏处：需要每隔一段时间备份一次。

### backup

```bash
# 原来
rm mackup/file
mv home/file mackup/file
link mackup/file home/file

# 现在
rm mackup/file
cp home/file mackup/file
```

### restore

```bash
# 原来
rm home/file
link mackup/file home/file

# 现在
rm home/file
copy mackup/file home/file
```

### uninstall

删除该功能

## 安装

```bash
git clone git@github.com:zqhong/mackup.git
cd mackup
python setup.py
```

## 命令行使用

* `mackup -h`：显示帮助
* `mackup backup`：备份配置文件
* `mackup restore`：恢复配置文件
* `mackup list`：列出 Mackup 支持备份的应用

## 配置说明

参考：[doc/README.md](doc/README.md)

## 支持的同步方式

- [Dropbox](https://www.dropbox.com/)
- [Google Drive](https://drive.google.com/)
- [Copy](https://www.copy.com/)
- [iCloud](http://www.apple.com/icloud/)
- [Box](https://www.box.com)
- file_system

## 支持同步的应用

参考：[mackup/applications/](mackup/applications/)
