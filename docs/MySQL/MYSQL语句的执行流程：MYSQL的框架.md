# 参考 
[执行一条 select 语句，期间发生了什么？ | 小林coding (xiaolincoding.com)](https://xiaolincoding.com/mysql/base/how_select.html#mysql-%E6%89%A7%E8%A1%8C%E6%B5%81%E7%A8%8B%E6%98%AF%E6%80%8E%E6%A0%B7%E7%9A%84)

# MySQL的框架 
![[Pasted image 20231227172830.png]]
注意，在8.0以后，MySQL不再使用查询缓存。
可以看到， MySQL 的架构共分为两层：**Server 层和存储引擎层**。
**Server 层负责建立连接、分析和执行 SQL**。
**存储引擎层负责数据的存储和提取**。
# SQL的执行流程 
## 连接器



