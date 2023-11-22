# 显微切片机硬件设计

垂直轴采用35步进电机，同步带传动，直线导轨滑动。
水平轴采用28BYJ-48减速步进电机，丝杆传动，在3D打印导轨滑动。
兼容市场上的包埋盒，采用009RD刀片。

# 恢复FreeCAD文档
FreeCAD文档已经进过zip压缩，为了方便git管理，缩小变更集尺寸，在git仓库只储存解压后的文件
### 从仓库文件中还原，供FreeCAD打开
`./zippey.py d < model.FCStd.zippey > model.FCStd`
### 编码成zipper格式，供git提交
`./zippey.py e < model.FCStd > model.FCStd.zippey`

方法来源：[levity0815/freecad_git_tryout](https://github.com/levity0815/freecad_git_tryout)
为了压缩带UTF-8字符的Document.xml文件，修改zippey.py文件了
