# Mackup

配置文件备份工具

## 安装
```bash
git clone git@github.com:zqhong/mackup.git
cd mackup
python setup.py
```

## 使用
* `mackup -h`：显示帮助
* `mackup backup`：备份配置文件
    * rm mackup/file
    * cp home/file mackup/file
* `mackup restore`：恢复配置文件
    * rm home/file
    * copy mackup/file home/file
* `mackup list`：列出 Mackup 支持备份的应用


## 支持的同步方式

- [Dropbox](https://www.dropbox.com/)
- [Google Drive](https://drive.google.com/)
- [Copy](https://www.copy.com/)
- [iCloud](http://www.apple.com/icloud/)
- [Box](https://www.box.com)
- 同步到目录
