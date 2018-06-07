#### 用例： 课程列表
- 权限： 学生/老师登录后可以看到。
- 功能： 返回所有课程的列表。
- API请求地址： 接口基本地址/v1/api/getCourses
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 36,
      "data": [
          {
          "ID":19,
          "COURSE_NO":"41052",
          "COURSE_NAME":"信息系统",
          "TERM_ID": "大三第2学年",
          "STATUS":"1",
          "STU_NO":"15",
          "TCH_NO":"2"
          "ADDTIME": "2018-05-28 17:48:01",
          ...
          },
          
          {
          ...其他课程
          }
      ]
  }

```
- 返回参数说明：

参数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回课程数量
data | 所有课程的数组
ID | 	数据库自增
COURSE_NO |课程编号
COURSE_NAME |课程名称
TERM_ID |学期编号
STU_NO |学生编号
TCH_NO |老师编号
STATUS |是否正常
ADDTIME | 增加日期


