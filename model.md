# 课程表 course

|字段名|数据类型|约束|
|-|-|-|
|course\_id|int|主键，自增，非空|
|course\_name|varchar(50)|非空|
|credit|int|非空|
|tea\_id|int|外键，关联教师表|

# 选课成绩表 score
dev-zhangsan

|字段名|数据类型|约束|
|-|-|-|
|id|int|主键，自增|
|stu\_id|int|非空，外键→学生表|
|course\_id|int|非空，外键→课程表|
|score|decimal(5,2)|成绩|



\# 数据库设计文档



\## 1. 学生表 (student)

\- student\_id: VARCHAR(20), 主键

\- name: VARCHAR(50), 非空

\- gender: ENUM('男','女')



\## 2. 教师表 (teacher)

\- teacher\_id: VARCHAR(20), 主键

\- name: VARCHAR(50), 非空

=======
字段名      | 数据类型     | 约束
-----------|------------|-----------------
id         | int        | 主键，自增
course_id  | int        | 非空，外键→课程表
score      | decimal(5,2)| 成绩
main
