# Python

```bash
# 导出库
pip freeze > requirements.txt

# 导出项目库
pip install pipreqs
pipreqs /path/to/project
```

# Markdown

```
# Github Readme
<h1 align="center">Python_YYDS</h1>
<p align="center">
    <img alt="Static Badge" src="https://img.shields.io/badge/Auth-Jeremy-brightgreen">
    <img alt="Static Badge" src="https://img.shields.io/badge/Version-v1.1.0-blue">
    <img alt="Static Badge" src="https://img.shields.io/badge/ILovePython-pink">
</p>

# 换页
<div style="page-break-after: always;"></div>
```

# Git

```bash
# 全局设置
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# 仅当前仓库
git config user.name "Your Name"
git config user.email "you@example.com"

# 克隆
git clone https://github.com/JeremyChim/Py.git

# 暂存
git add .

# 提交
git commmit -m "提交内容"

# 检查
git status

# 推送
git push -u origin main

# 撤销暂存
git reset .

# 更改仓库url
git remote set-url origin https://github.com/JeremyChim/D2FUN.git

# 切换项目远程地址为 SSH 协议
# 将 your-username 和 your-repo 替换为实际的 GitHub 用户名和仓库名
git remote set-url origin git@github.com:your-username/your-repo.git


```

# 配置ssh

```bash
# 是否已存在 SSH 密钥
ls -al ~/.ssh

# 生成新的 SSH 密钥（如果没有）
ssh-keygen -t ed25519 -C "jer888chim@outlook.com"

# 启动SSH代理
eval "$(ssh-agent -s)"

# 将新生成的SSH密钥添加到代理
ssh-add ~/.ssh/id_ed25519

# 查看公钥内容，复制
cat ~/.ssh/id_ed25519.pub

# 登录 GitHub → Settings → SSH and GPG keys → New SSH key
# 粘贴公钥内容，添加标题（如 My Laptop），点击 Add SSH key

# 测试连接
ssh -T git@github.com

# 成功信任后，你应该会看到类似这样的确认信息：
# Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
# Hi jer888chim! You've successfully authenticated, but GitHub does not provide shell access.
```
