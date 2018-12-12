# 创建一个github 仓库通常要做的事情包括下面的作业
···

…or create a new repository on the command line
 
echo "# rhels8_study_notes" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:824380210/rhels8_study_notes.git
git push -u origin master
…or push an existing repository from the command line
 
git remote add origin git@github.com:824380210/rhels8_study_notes.git
git push -u origin maste


···
