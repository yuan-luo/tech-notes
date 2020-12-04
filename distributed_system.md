Google Spanner Notes:

Spanner的事务分为读写事务，只读事务(预先申明的快照隔离事务)以及快照读。

Spanner 用的 TrueTime 技术，依赖于原子钟和卫星来实现单调递增的全局时间戳。

Spanner使用Paxos协议在多个副本间同步redo日志，从而保证数据在多个副本上是一致的。Google的工程师钟情于Paxos协议，Chubby、Megastore和Spanner等一系列产品都是在Paxos协议的基础上实现一致性的。




