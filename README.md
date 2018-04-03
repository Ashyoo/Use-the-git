# Use-the-git

## git

* 查看修改用户名和邮箱

```
git config user.name ===> 查看名称
git config user.email ===> 查看邮箱

git config --global user.name "xxx"  ===>  修改名称
git config --global user.email "xxx"  ===>  修改邮箱
```

* 删除文件或文件夹

```
git rm (文件名)
```

* 将项目clone下来之后，使用 npm install 或 yarn install 指令安装依赖

* clone之后使用指令 **git branch -a** 查看分支

```
      master // 当前分支（master：主分支）
      remotes/origin/HEAD -> origin/master
      remotes/origin/develop
      remotes/origin/master
```

* 切换分支

```
$ git checkout <分支名>
```

* 关联主分支

```
$ git remote add (分支名) (url)
```

* 删除 remote 分支

```
git remote remove <分支名称>
```

## git 提交注释编写规范

* Commit Message 提交类型

> Commit Message 第一行的提交类型必须是以下类型之一:<br/>：feat, fix,docs,style,refactor,perf,test,chore。

1. feat -- 实现新功能(feature)
> 当新需求或新功能的实现完成并测试通过时，开发人员需提交该部分变更的代码，并且按照上述的Commit Message格式编写提交注解。E.g: feat: add listView components to bill search page

2. fix -- 解决bug
> 当Bug修复完成并确认已经彻底解决时，开发人员需提交该部分变更的代码，并且按照上述的Commit Message格式编写提交注解。 Example 1: fix: when submit button has ever been triggered, do not trigger again.(#1871) Example 2: fix(pp): fix the NullPointException when updating bill.

3. docs -- 只针对文档(documention)变更
> 如果提交的改动只是针对文档的变更，则提交类型可以设为docs，E.g: docs: add the document of Git Commit Message Guideline

4. style -- 代码样式(style)变更(格式化代码，不影响代码原意)
>如果提交的改动只是针对代码样式或者格式的变更，则提交类型可以设为'style'， E.g: style: reformat service layer code

5. refactor -- 代码重构(refactor)(既不是解决bug也不是实现新功能)
> 如果提交的改动是针对代码重构的，则提交类型可以填写为'refactor', E.g: refactor : refactor default search function

6. test -- 添加缺少的测试(test)代码
> 添加的代码为测试相关的代码，则提交类型可以填写为'test'， E.g: test: add unit test for user login function

7. perf -- 优化系统性能(performance)
> 若提交的改动是针对系统性能的优化的，则提交类型填写为'perf'，E.g: perf: improve the performance of filtering the required bill list

8. chore -- 针对构建过程或者辅助工具的变更 
> chore:日常零碎变更，这里主要是针对构建过程、辅助工具、抑或是其他无关主题代码的变更。E.g: chore: add css preprocessor trees

