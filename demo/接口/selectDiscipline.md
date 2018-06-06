# 接口：selectDiscipline  [返回](../README.md)
用例： [选择课程](../用例/选择课程.md)
- 功能：
    老师和学生进行选择课程。   
  
 - 权限：
     学生/老师：先登录，并且老师先选择课程，学生的选课链接方可打开
    
- API请求地址： 
    http://202.115.82.8:1522/v1/api/getUserSubject

- 请求方式 ：
    GET  

- 请求参数说明:        
    请求有三个个参数：userId、termId、disciplineId，userId参数为用户Id确定用户信息，以便后台查找该用户的相关数据信息。termId确定学期，进一步筛选课程。disciplineId确定选择的哪一门课程。
    
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