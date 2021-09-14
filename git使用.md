仓库地址：https://github.com/ruoxiaobai/lyd.git
token验证：
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
git上传步骤
	创建文件夹,使用git init 将文件夹初始化为本地仓库

![image-20210914153254942](../AppData/Roaming/Typora/typora-user-images/image-20210914153254942.png)

​	将需要上传的文件放入到该文件夹,再使用 git add 文件 -->git commit -m "描述" -->将文件添加到本地仓库,add可以添加多次即多个文件,commit提交一次即可

![image-20210914153312718](../AppData/Roaming/Typora/typora-user-images/image-20210914153312718.png)

​	再将远程源设置,即将自己的github仓库连接上(注意认证需要token,原先是不需要的)

由于设置过修改远程源代码也复制上

![image-20210914153357228](../AppData/Roaming/Typora/typora-user-images/image-20210914153357228.png)

修改远程源地址 git remote set -url origin https://token名@github.com/用户名/仓库名.git

![image-20210914153446165](../AppData/Roaming/Typora/typora-user-images/image-20210914153446165.png)



​	操作:git remote add origin https://github.com/token/用户名/仓库名.git-->在上方



​	修改分支:注意分支需要一致-->git branch -M 名称

![image-20210914153346703](../AppData/Roaming/Typora/typora-user-images/image-20210914153346703.png)	查看状态:git status
	上传操作:git push -u origin 分支名
注意如果上传失败(出现下方问题)需要设置:git config --global http.sslVerify 'false'

![image-20210914153548068](../AppData/Roaming/Typora/typora-user-images/image-20210914153548068.png)

成功上传

![image-20210914153614997](../AppData/Roaming/Typora/typora-user-images/image-20210914153614997.png)