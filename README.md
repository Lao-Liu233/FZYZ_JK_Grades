# FZYZ_JK_Grades

## 项目介绍

用于查询FZYZ官网成绩及APP“JK同学”内成绩的API及前端网站。

## 部署教程

### 部署开发/测试环境

需要安装的库：

Python3,pip3 ： 略；

`pip3 install Django beautifulsoup4 requests  ` 

开启测试Server ：

`python3 manage.py runserver 0.0.0.0:8000`

### 部署生产环境

[参见runoob](https://www.runoob.com/django/django-nginx-uwsgi.html)

## API参数

### fzyz/

用户名 ： 'user':'username',

密码 ： 'passwd':'password',

考试id ： 'exam':'exam_Id';

高一/二/三总评3704,卷面3703

### JK/

用户名 ： 'user':'username',

密码 ： 'passwd':'password',

学科id ： ‘subject’:'subject';

数学1；语文2；英语3；物理4；化学5；生物6；政治7；历史8；地理9；信息技术10；理综11；文综12。

## 已知问题

前端仅支持FZYZ官网查询功能，且查询API时需跳转其他地址；

FZYZ官网仅能查询高三年级第一学期期末考卷面成绩，且返回的是未经解析的HTML；

JK仅能返回该科目全部考试成绩，且返回的是未经分析的JSON。

## TO DO LIST

- [ ] 补全FZYZ官网查询科目/考试
- [ ] 补全JK查询科目/考试
- [x] 构建能用的前端
- [ ] 构建美丽的前端
- [x] 将代码部署服务器

## 我们需要？

能构建Ajax前端的人（需要jQery等JS基础）；

能设计美丽前端的人（需要框架基础）；

能补全API查询范围的人（希望高一/高二有兴趣的同学能提供开发所需要的数据）；

发现任何问题后开issue反馈的人；

有兴趣提交任何代码的人。