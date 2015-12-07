===Git简介===

Git是版本控制管理工具，作者Linus

git log 命令选项

![git-log.png](https://github.com/zaifeng/GitStudy/blob/master/images/git-log.png "option words")

<table>
    <tr>
        <td>a</td><td>b</td>
    </tr>
    <tr>
        <td>a</td><td>b</td>
    </tr>
    <tr>
        <td>a</td><td>b</td>
    </tr>
</table>


git status -s 可以查看系统那些文件做了那些修改

例如：

$git status -s
M hello.md

$git diff 用于查看difference,显示的格式正是Unix通用的diff格式

$git diff 无参数情况，表示工作区和索引区对比

$git diff --cached 表示索引区和版本控制区对比


