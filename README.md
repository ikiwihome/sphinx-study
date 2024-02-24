# Sphinx和reStructureText手册

网页浏览地址：<https://sphinx-rst-manual.readthedocs.io>

## 如何使用

### 文件目录说明

```
│
├───docs                        # 工程文档和配置脚本文件夹，install和make脚本都在这里
│   │
│   ├───_static                 # html样式css和js文件夹
│   │
│   ├───_templates              # html页面模板文件夹
│   │
│   ├───latex_templates         # latex样式模板(生成pdf的样式)
│   │   │
│   │   └───fonts               # pdf字体文件夹
│   │
│   └───source                  # 工程文档存放文件夹
│       │
│       ├───_static             # 文档自定义的html样式，默认空
│       │
│       ├───_templates          # 文档自定义的html页面元素，默认空
│       │
│       ├───conf.py             # sphinx的配置文件
│       │
│       └───index.rst           # 文档目录文件，必须有，否则报错
│
└───env                         # windows python本地环境文件夹，双击install.bat会解压python环境

```

所有的源文件都存放在 docs/source 文件夹下：

- 配置文件为 conf.py 文件
- 各章节目录为各个 index.rst 文件
- 各章节页面为各个 xxx.md 文件

如需修改，**请直接修改 /source 文件夹下的相应文件。**

### 前提
- Linux 环境：python >3.7，运行docs/install.sh安装
- Windows 环境：双击docs文件夹下的install.bat解压python压缩包
- 先执行```cd docs``` 命令切换到docs目录下
- 生成pdf需要安装MikTex或者TexLive，以及Perl

### 创建html

```
make html
```

### 创建pdf

```
make pdf
```

### 创建html和pdf

```
make all
```

### 清空_build文件夹

```
make clean
```

## License

MIT