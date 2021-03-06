# 实验二：用例建模


##1.实验目标1
 - 确定本门课程的个人选题
 - 在个人选题添加个人的功能介绍
 - 画出个人选题系统的用例图
 - 编写用例规约
 
##2.实验内容

 - 提交issue选题商品购物秒杀系统 #629
 - 确定该系统的功能需求
 - 使用StarUML画出用例图
 - 创建用例规约
 - 撰写实验报告二
 - 提交实验
 
##3.实验步骤

 - 确定选题：商品购物秒杀系统 # 629
	 - 细化功能需求
	 	- 1.抢购秒杀商品
	 	- 2.查看秒杀商品
 - 根据选题画出用例图
	 - 在starUML上创建一个商品购物系统
	 - 添加消费者用例
	 - 根据功能需求建出用例图
	 - 导出用例图
 - 填写用例规约
 - 将用例图和实验文档merge到本地仓库
 - 提交实验报告二
 
##4.实验结果

![用例模型图](./Lab2_UseCaseDiagram.jpg)  

 	 图一：商品秒杀系统的用例图

## 表1：查看秒杀商品规约  

用例编号  | UC01 | 备注  
-|:-|-  
用例名称  | 查看秒杀商品  |   
前置条件  |  登录成功    | *可选*   
后置条件  | 消费者进入商品秒杀购物首页     | *可选*   
基本流程  | 1. 消费者点击查看秒杀商品详情；  |*用例执行成功的步骤*    
~| 2. 系统显示秒杀商品详情页面；  |   
~| 3. 消费者输入商品名称，点击完成按钮；  |
~| 4. 系统检查商品名称不为空，查询商品信息。  |    
~| 5. 系统显示秒杀商品信息。  | 
扩展流程  | 4.1 系统检查发现商品名字为空，**提示“商品名称不能为空”**；  |*用例执行失败*   
扩展流程  | 4.2 系统检查发现商品信息不匹配，**提示“查无此商品”**；  |*用例执行失败*   *用例执行失败*   


## 表2：抢购秒杀商品

用例编号  | UC02 | 备注  
-|:-|-  
用例名称  | 抢购秒杀商品  |   
前置条件  | 消费者进入秒杀商品购物列表     | *可选*   
后置条件  |   秒杀活动未结束且商品数量足够 | *可选*   
基本流程  | 1. 消费者点击**抢购商品**链接；  |*用例执行成功的步骤*    
~| 2. 系统显示抢购秒杀商品信息页面  |   
~| 3. 系统**检查到**确认秒杀商品库存有余、活动是否结束  |   
~| 4. 商品库存扣除成功，创建订单，返回购物结果   |  
扩展流程  | 3.1 系统检查发现商品库存不足或活动已结束，**提示“商品库存不足或活动已结束”**；  |*用例执行失败*      

