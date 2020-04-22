# python 报错

## pip报错

安装、更新第三方库报错timeout的解决方法

* 设置延迟时间

```
pip --default-timeout=1000 install ...
```

* 使用镜像站

```
临时使用清华源
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple ...
```

## pyinstaller报错

用图片打包程序时，出现了报错：AttributeError: module 'win32ctypes.pywin32.win32api' has no attribute 'error'。这是因为打包的图片格式不对，图片格式改为ico。

改为ico后，又出现的这样的报错：struct.error: unpack requires a buffer of 16 bytes。解决方法：“http://ico.duduxuexi.com/” 将图片生成为16\*16的图标文件。
