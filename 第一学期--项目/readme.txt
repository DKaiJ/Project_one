通用框架说明：
	1.dao包已经提供了DBHelper类，包括增删改查及查询统计函数的方法
		但要注意，如sql参数有特殊类型的，要修改doParams()， findAll().
	2.bean包：	放实体类，与数据库表对应
	  biz包：	业务，如结账，转账，。。。。诸如此类的要同时操作n张表的操作就叫业务。
	  dao包：	DBHelper足以。
	  ui包：		放swt的界面。
	  		子包：	以模块命名子包。
	  				admin
	  				product
	  utiles包：	各种工具神器。
	  pic包：	放项目所需的图片，图片最好是英文拼写，不能用中文。
	  
test：是一个source folder，用于放置测试代码，以后发布不用管。
product.sql：是项目的数据库创建脚本，可以有多个，
				create.sql：表示创建库，表，关系，约束的脚本
				data.sql：	表示插入测试数据的脚本