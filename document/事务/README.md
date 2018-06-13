##**关于事务需要了解的内容有：**

- 事务的四大特性：
    
    1. 原子性（A Atomicity）
    2. 一致性（C Consistency）
    3. 隔离性（I Isolation）
    4. 持久性（D Durability）
    
- 事务的四大隔离级别：

    1. 读已提交（Read Committed）
    2. 读未提交（Read Uncommitted）
    3. 可重复读（Repeatable Read）
    4. 可序列化读（Serializable）
    
    需要了解每种隔离级别的优缺点,了解脏读、可重复读、幻读概念
    
- 事务的七大传播机制

    1. REQUIRED
    2. NOT_SUPPORTED
    3. REQUIREDS_NEW
    4. MANDATORY
    5. NEVER
    6. SUPPORTS
    7. NESTED
    
事务的四大隔离级别和七大传播机制主要是针对spring中的事务控制，spring本身并不控制事事务，而是提供了多种事务管理器，从而将事务管理的职责转交给Hibernate或者MyBatis等持久化机制所提供的相关平台框架的事务来实现。