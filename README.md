# [GIT]开发者角色使用教程  
  
#### 下载项目.  
  
1.把项目下载到自己的本地文件夹(cd 到想要存储工程的文件夹)  
  
  `git clone https://gitee.com/HuaLongXunDaYiDong/gitCourse.git`  
  
  
  
#### 修改后更新项目  
  
1.设置仓库地址    
  
  `git remote add origin https://gitee.com/HuaLongXunDaYiDong/gitCourse.git`  
  
  
2.执行对比操作,对比云端代码与本地代码的差异  
  
  `git add -u`  
  
3.执行代码更新注解     
  
  `git commit -m "更新测试"`  
  
4.执行上传更新操作  
  
  `git push -u origin master`  
  
#### 错误汇总  
  
##### 1.如果 [设置仓库地址出错]`git remote add https:...`  
*   错误描述：  
>git提示出错信息：fatal:remote origin already exists.  

*   解决(先删除之前设置远程仓库地址)  
  
>` git remote rm origin`  
  
##### 2.如果执行 [上传更新操作] `git push -u origin master` 出错  
  
*   解决(一般出现此问题是因为云端上面有本地未同步的代码或者文件，所以先执行一下命令同步一下，再从新 push 尝试)  
  
>`git pull origin master`


##### 2.推送的时候不可使用 git push -f origin master    其中 -f 是强制推送功能！  
  
