Markdown ,文本修饰语言,用特殊符号修饰正文效果<br>
# GitHub 使用笔记

## 关键字查询
- `awesome`：在此标签类别中查询项目。
- `python tutorial`：查询资料、书籍、文档。
- `socket sample`：查询对应技术的代码样本。

## GitHub 三要素
### Repository（仓库）
仓库是GitHub项目管理存储的基本单位。一个仓库中存储一个项目，一个用户可以拥有多个仓库。仓库一般分为public（公开）和private（私有）。

### Commit（提交）
程序员在整个开发周期中，有大量的对代码资源的**迭代**和修改，都可以通过commit的方式进行记录，便于程序员**回溯**代码。即使这些代码被删除，提交也可以帮助使用者观察整个工程的开发流程以及设计流程。

### Branch（分支）
在仓库中可以包含多个分支，分支才是代码文件的第一存储单位。默认的仓库主分支为`master`或`main`。分支不仅可以管理代码存储，还便于多人协作开发仓库内容。

## 其他要素
- **Code**：资源存储，代码资源，二进制项目管理版本，许可证等。
- **Issues**：使用时遇到的bug可以进行提交，等待反馈。
- **README**：使用Markdown语言编写的工程自述文件，包括开发进度、版本更新、使用介绍等。
- **LICENSE**：许可证，如GPL 2.0、3.0、Apache 2.0、MIT等，给使用者最大使用权限以及最少的限制。
- **Git 软件**：分布式版本控制系统，用于仓库管理。

## 设备认证与代码管理
1. 如何让网站的账户与设备绑定，后续可进行代码的管理，包括上传和下载。
   - `git init`：创建本地仓库。
   - `git config --list`：查看Git的配置文件。
   - `git config --global user.email "邮箱"`：配置全局用户邮箱。
   - `git config --global user.name "用户名"`：配置全局用户名。

### SSH 远程访问
- `ssh-keygen -t rsa -C "注册邮箱"`：创建本地密钥。
- 在对应的**目录**查找密钥文件`rsa.pub`，复制内容。
- 粘贴到GitHub的SSH key设置中。
- `ssh -T git@github.com`：测试关联是否成功。

### Git命令
- `git remote add origin "ssh地址"`：为SSH仓库地址创建别名为`origin`。
- `git remote remove origin`：删除`origin`别名。
- `git add`：添加内容到暂存区。
- `git rm`：删除本地文件并提交到仓库。
- `git restore`：恢复被删除的文件（如果仓库中存在）。

### 分支Branch
- 关于分支的相关命令，包括创建分支、选择分支、合并分支等。

## Markdown 语言
GitHub可以使用Markdown语言编写README文件，这是一种文本修饰语言。

#标题修饰符(一级标题)
##(二级标题)
###(三级标题)

##正文内容
##修饰正文
*一段测试文本*
**一段测试文本**
***一段测试文本****

