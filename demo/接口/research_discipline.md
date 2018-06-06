# 接口：research_discipline  [返回](../README.md)
用例： [查找课程](../用例/查找课程.md)
- 功能：
    老师和学生进行查找课程  
  
 - 权限：
     学生/老师：先登录
    
- API请求地址： 
    http://202.115.82.8:1522/v1/api/research_discipline

- 请求方式 ：
    GET  

- 请求参数说明:        

     |参数名称|说明|
      |:---------:|:--------------------------------------------------------|      
      |id|学生学号或者老师的工号，由type决定。|
      |password|用户的密码，不是原文，是加密后的字符串| 
      |type|用户类型，学生或者老师|
      |terms_id|学期编号|
      |discipline_id|课程编号|
    
- 返回实例：

        {
            "status": true,
            "discipline_id":"1",
            "discipline_name":"软件系统分析与设计",
            "discipline_time":"周一上午1、2节课"
            "discipline_population":"60"
            "discipline_hour":"48"
        }
  
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |discipline_id|课程编号|
  |discipline_name|课程名称|
  |discipline_time|课程时间|
  |discipline_poplution|课程人数|
  |discipline_hour|课时|
