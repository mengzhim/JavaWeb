#                                             MyBatis

### 简介

- MyBatis是一款持久层（负责将数据保存到数据库的那层代码）框架（半成品软件），用于简化JDBC开发

### MyBatis简化JDBC：

- 硬编码（配置文件完成）
  - 注册驱动，获取连接
  - SQL语句
- 操作繁琐（自动完成）
  - 手动设置参数
  - 手动封装结果集

### Mapper代理开发

1.定义与SQL映射文件同名的Mapper接口，并将Mapper接口和SQL映射文件放在同一目录下

2.设置SQL映射文件的namespace属性为Mapper接口限定名

3.在Mapper接口中定义方法

4.编码

### MyBatis核心配置文件

- environments：配置数据库连接信息，可以配置多个environment，通过default来切换environment

### MyBatis步骤

1.获取SqlSessionFactory对象

2.获取SqlSession对象

3.获取Mapper接口代理对象

4.执行Mapper中的方法

5.释放资源，sqlSession



### 参数占位符

- #{}：会被替换为？，防止SQL注入
- ${}：拼接SQL语句，存在SQL注入



### 注解开发

- 查询：@Select
- 添加：@Insert
- 修改：@Update
- 删除：@Delete

注解完成简单功能，配置文件完成复杂功能

@Select("select * from tb_user where id = #{id}")

public User selectById(int id);