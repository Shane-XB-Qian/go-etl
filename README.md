# go-etl

go-etl将提供的etl能力如下：

1. 主流数据库的数据抽取以及数据加载的能力，这个计划在storage包中实现
2. 类似datax的数据同步能力，这个计划在datax包中实现
3. 数据库间的数据校验能力，这个计划在libra包中实现
4. 以mysql sql语法为基础的数据筛选、转化能力，这个计划在transform包中实现（计划中）

## plan

### datax

- [x] 实现datax的同步框架，不包含监控以及流控模块
- [x] 单元测试datax的同步框架，不包含监控以及流控模块
- [ ] 系统测试MySQL数据库间的同步
- [ ] 实现监控以及流控模块,并单元测试（延后实现）

### storage

- [x] 实现数据库的数据抽取以及数据加载框架以及MySQL数据库的相应接口
- [ ] 单元测试实现数据库的数据抽取以及数据加载框架以及MySQL数据库的相应接口
- [ ] 实现MySQL基于datax的同步接口，并单元测试
- [ ] 实现MySQL数据库的libra接口并单元测试

### libra

- [ ] 实现libra的数据校验框架
- [ ] 单元测试libra的数据校验框架
- [ ] 系统测试MySQL数据库间校验

### transform

目前计划中













