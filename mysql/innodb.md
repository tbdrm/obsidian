
![](Pasted%20image%2020230831154905.png)
innodb内存区组成
- redolog buffer
- 缓存页、数据页
- change buffer（非唯一非聚簇索引）
- AHI

关键特性
![](Pasted%20image%2020230901140615.png)

文件
- 错误日志
- 查询日志
- 慢查询日志
- 二进制日志
	- 默认ROW格式，记录所有变化，磁盘空间占用更大，但是不会有部分语句问题，例如rand和uuid函数
	- 以前是STATEMENT，记录语句

逻辑存储结构
![](Pasted%20image%2020230901155352.png)