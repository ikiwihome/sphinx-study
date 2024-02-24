# Sphinx和reStructureText手册

网页浏览地址：<https://sphinx-rst-manual.readthedocs.io>

## 如何使用

所有的源文件都存放在 docs/source 文件夹下：

- 配置文件为 conf.py 文件
- 各章节目录为各个 index.rst 文件
- 各章节页面为各个 xxx.md 文件

如需修改，**请直接修改 /source 文件夹下的相应文件。**

### 前提
- python >3.7
- cd docs
- pip install -r requirements.txt
- MikTex或者TexLive，以及Perl

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

### 清空生成文件

```
make clean
```

## License

MIT