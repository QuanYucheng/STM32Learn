2025.7.29
（一）今日任务
1、安装VSCode，再安装git，git编辑器选择VSCode，git的鼠标右键扩展菜单不要勾选git GUI，仅勾选git bash，在VSCode安装gitLens和git graph插件。
2、注册st账号，在st官网下载STM32CubeMX，安装STM32CubeMX，运行STM32CubeMX并创建一个STM32F103C8T6项目，生成项目代码。
3、注册git账号，并创建一个名为STM32Learn的仓库，右键STM32CubeMX目录，通过VSCode打开，在终端通过指令创建git仓库，并提交到github上。
（二）执行难点
任务3中使用的创建库，上传等代码指令的学习与使用。
其代码如下：
cd MyProject                     # 进入你的项目文件夹
git init                         # 初始化本地仓库
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
echo "# 这是我的项目" > README.md
git add .                        # 添加所有文件
git commit -m "初始化项目"
git remote add origin https://github.com/yourname/MyProject.git
git push -u origin main          # 推送代码到 GitHub
逐步执行完成目的

设置代理（如果有），端口需要根据机场设置
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890

取消代理的设置
git config --unset http.proxy
git config --unset https.proxy