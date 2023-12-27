<h1>git 远端操作</h1>
<h2>git 基本命令</h2>

- <code>git init</code> 初始化一个全新的 Git 存储库并开始跟踪现有目录。 它在现有目录中添加一个隐藏的子文件夹，该子文件夹包含版本控制所需的内部数据结构。

- <code>git clone</code> 创建远程已存在的项目的本地副本。 克隆包括项目的所有文件、历史记录和分支。

- <code>git add</code> 暂存更改。 Git 跟踪对开发人员代码库的更改，但有必要暂存更改并拍摄更改的快照，以将其包含在项目的历史记录中。 此命令执行暂存，即该两步过程的第一部分。 暂存的任何更改都将成为下一个快照的一部分，并成为项目历史记录的一部分。 通过单独暂存和提交，开发人员可以完全控制其项目的历史记录，而无需更改其编码和工作方式。

- <code>git commit</code> 将快照保存到项目历史记录中并完成更改跟踪过程。 简言之，提交就像拍照一样。 任何使用 git add 暂存的内容都将成为使用 git commit 的快照的一部分。

- <code>git status</code> 将更改的状态显示为未跟踪、已修改或已暂存。

- <code>git branch</code> 显示正在本地处理的分支。

- <code>git merge</code> 将开发线合并在一起。 此命令通常用于合并在两个不同分支上所做的更改。 例如，当开发人员想要将功能分支中的更改合并到主分支以进行部署时，他们会合并。

- <code>git pull</code> 使用远程对应项的更新来更新本地开发线。 如果队友已向远程上的分支进行了提交，并且他们希望将这些更改反映到其本地环境中，则开发人员将使用此命令。

- <code>git push</code> 使用本地对分支所做的任何提交来更新远程存储库。

<h2>git 自用模板</h2>

<code>
    
    git init

    git add README.md

    git commit -m "first commit"

    git branch -M main

    git remote add origin https://github.com/sufeng1216/deep_learning_notes.git

    git push -u origin main

</code>