#  鍒涘缓涓??涓猤ithub 浠撳簱閫氬父瑕佸仛鐨勪簨鎯呭寘鎷笅闈㈢殑浣滀笟
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
# 绗竴娆℃帹閫佸け璐ュ彲浠ュ皾璇 git push -u -f origin master
##  -f 鏄己鍒舵帹閫侊紝寰堝ぇ鐨勫師鍥犳槸浣犵殑搴撴病鏈夊悓姝ワ紝濡傜洰鏍囨湁浜嗘柊鏂囦欢锛屼絾浣犵殑娌℃湁锛屽鑷姩鐢熸垚鐨凴EADME.md
```
Warning: Permanently added the RSA host key for IP address '13.229.188.59' to the list of known hosts.
No refs in common and none specified; doing nothing.
Perhaps you should specify a branch such as 'master'.
error: failed to push some refs to 'git@github.com:824380210/rhels8_study_notes.git'
[root@test rhels8_study_notes]# git push -u -f origin master




```
