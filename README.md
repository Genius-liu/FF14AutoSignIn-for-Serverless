##  可以使用腾讯云云函数的FF14 国服官网自动签到脚本

*补全了需要的依赖库并修复了几处错误*  
*核心来自https://github.com/renchangjiu/FF14AutoSignIn *  
*特别感谢@renchangjiu 大佬*  

#1.作用  
使用腾讯云云函数实现每日自动在云端签到


#2.使用前
在本地修改config.py中的内容（上传后用云端编辑器修改也可以）


#3.安装
3.1在腾讯云新建一个空的云函数（地区推荐选择国内）, 函数名称随便写, **运行环境Python3.7**，**执行方法填写 `main.index`**, 并上传函数代码。
![image](https://github.com/Genius-liu/FF14AutoSignIn-for-Serverless/blob/main/image/3.1.png)

3.2建议将执行超时时间设置长一点，推荐设置为30-60秒
![image](https://github.com/Genius-liu/FF14AutoSignIn-for-Serverless/blob/main/image/3.2.png)

3.3设置定时触发器, 触发方式：`定时触发`, 触发周期：`自定义触发周期`, Cron表达式：`0 0 8 * * * *` (北京时间每天早上8点触发一次，可以自己随便设定）
![image](https://github.com/Genius-liu/FF14AutoSignIn-for-Serverless/blob/main/image/3.3.png)


#4.用法
![image](https://github.com/Genius-liu/FF14AutoSignIn-for-Serverless/blob/main/image/4.1.png)
![image](https://github.com/Genius-liu/FF14AutoSignIn-for-Serverless/blob/main/image/4.2.png)
