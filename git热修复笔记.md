# git 热修复

1、先新建一个  Hot_br20220630  分支

2、然后选择从   master   分支上来取 （合并），不能从Dev分支上取，因为dev分支已经在做下一个版本的功能了

3、之后我们在Hot_br20220630分支上进行修复，修复完交测试，测试完进行代码合并

4、然后将分支先切换到master分支，并将Hot_br20220630分支的代码合并到master分支上来   

命令是 ：

​	1、切换分支：git checkout 《分支名》

​	2、合并：git merge Hot_br20220630 分支       合并到master分支上	

​	3、项目打包：npm run build

​	4、布置服务器（把你master分支的代码放在服务器上）

​	5、最后切换到Dev分支上，然后将master分支的代码合并到Dev分支上