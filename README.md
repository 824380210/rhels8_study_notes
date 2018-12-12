# 创建一个github 仓库通常要做的事情包括下面的作业
```

…or create a new repository on the command line
 
echo "# rhels8_study_notes" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:824380210/rhels8_study_notes.git
git push -u origin master
…or push an existing repository from the command line
 
git remote add origin git@github.com:824380210/rhels8_study_notes.git
git push -u origin master


```
# 第一次推送失败可以尝试用这个命令git push -u -f origin master
## -f 是强制推送，很大的原因是你的库没有同步，如目标有了新文件，但你的没有，如自动生成的README.md

```
Warning: Permanently added the RSA host key for IP address '13.229.188.59' to the list of known hosts.
No refs in common and none specified; doing nothing.
Perhaps you should specify a branch such as 'master'.
error: failed to push some refs to 'git@github.com:824380210/rhels8_study_notes.git'
[root@test rhels8_study_notes]# git push -u -f origin master




```
