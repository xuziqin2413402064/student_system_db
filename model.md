# 课程表 course
字段名      | 数据类型     | 约束
-----------|------------|-----------------
course_id  | int        | 主键，自增，非空
course_name| varchar(50)| 非空
credit     | int        | 非空
tea_id     | int        | 外键，关联教师表

# 选课成绩表 score
字段名      | 数据类型     | 约束
-----------|------------|-----------------
id         | int        | 主键，自增
stu_id     | int        | 非空，外键→学生表
course_id  | int        | 非空，外键→课程表
score      | decimal(5,2)| 成绩
