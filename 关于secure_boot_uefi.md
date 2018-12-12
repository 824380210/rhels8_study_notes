# 什么是secure boot uefi
# 为了安全，要求在系统引导的内核，文件需要经过一个私有密钥的签名，经过这个私有密钥签名的内核确认是安全，只有签名的内核才能引导，这就是secure boot的基本思想
##
# 红帽的Beta 版本内核与GA 版本的内核的签名私有密钥是不一样的，因此，如果想让你的硬件支持beta内核 ，你需要将红帽的beta公钥加入到你的硬件( TPM )中去，这样才能识别由私有密钥签名的内核
# Machine Owner Key (MOK)这个工具负责将密钥加入到硬件中去
# 
```
0:      关闭secure boot
1:	#yum install kernel-doc
2:	# kr=$(uname -r)
3:	# mokutil --import /usr/share/doc/kernel-keys/${kr%.$(uname -p)}/kernel-signing-ca.cer
4:	输入密码
5:	重启系统
6:	按提示输入密码（步骤5的密码）
7:	启用secure boot	

9:	如果要删除密钥，执行下面的命令即可(注意要提供import时候提供的密码 )
10:	mokutil --reset
      
```
