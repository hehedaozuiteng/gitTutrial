# gitTutrial

# .gitignore 作用

里面表示的文件会再工作流程中被忽略并且不会追踪。

# 完整的一次工作流程

![img](git-command.jpg)

### 从远程仓库拉取自本地仓库

```bash 
git clone <link>

git clone git@github.com:hehedaozuiteng/gitTutrial.git

```

### checkout 至指定的分支

```
git branch   # 查看本地有几个branch
    * main    《=== 说明，只有一个分支 main
```

```
git branch branch_1   《=== 创建分支 1

git checkout -b branch_2  《==== 创建分支 2 并跳转至分支2

    Switched to a new branch 'branch_2'

git branch 

  branch_1
* branch_2   《==== 我们在 branch_2 下面 并且目前这个本地仓库有 3 个branch
  main

```

回到分支main
```
git checkout main
git branch

  branch_1
  branch_2   
* main

```

```
git checkout <branch name>
```

### 从工作区提交至本地仓库

```

git status 《===== 查看 git 当前情况

git add . 《==== 将所有的文件更改加入到staged 区域

git restore --staged . 《 === 将所有staged 区域的更改送回到working space

git add filename.type 《=== 将当个文件filename.type 加入到stage 中

git commit -m "message"

```

```

git log #查看历史commits

git diff <hash> #将目前的git和指定的commit 进行对比

git diff HEAD #将本地的working space 文件和branch最新的commit 进行对比

git diff HEAD^ #将本地的working space 文件和branch上一个最新的commit 进行对比

```


### 上传并同步本地分支

```

git pull --rebase

git push

```


