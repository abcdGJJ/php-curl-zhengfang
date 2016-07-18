## 正方教务系统获取实时成绩，成绩更新时发邮件提醒
#### 原理：
1. php模拟登录正方
2. 使用老司机的验证码识别工具。http://www.unique-liu.com/211.html
3. phpmailer发送邮件
4. crontab定时任务

#### 不足：
1. 验证码识别率低，需要缩短获取成绩间隔以便提高准确率
2. 无法做到动态更新`<td>`数量，需要修改代码，否则就会按照执行间隔不停的发送邮件。