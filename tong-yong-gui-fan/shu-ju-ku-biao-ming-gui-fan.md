# 数据库表名规范

1. 表名设计必须以模块名为开头，如能源管理（EMS\_）,质检（QC\_）,物流（LE\_）;
2. 主表名必须以主实体命名，如能源管理-测量点类型（EMS\_MEASUREPOINTTYPE）；
3. 子表命名分两种情况处理：
   1. 单子表：主表结尾加\_B，如EMS\_MEASUREPOINTTYPE\_B
   2. 多子表：主表结尾加子表代表性单词，如BD\_BOM\_OUTPUTS
4. 孙表命名与子表类似，不需要在子表表名后加后缀，以主实体表名后加后缀即可。









