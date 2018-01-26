# 强制字段命名规范

> _主键都是char\(36\)，外键是varchar2\(36\)._
>
>                                                         ---_ _**by WEI**



| 字段编码 | 字段名称 | 字段类型 | 是否可空 | 备注 |
| :---: | :---: | :---: | :---: | :---: |
| id | 主键 | char\(36\) | 否 | 不论主表子表，主键全部以id命名 |
| code | 编码 | varchar2\(50\) | 否 | 档案节点的编码名称必须按此规则命名 |
| name | 名称 | varchar2\(50\) | 否 | 档案节点的编码名称必须按此规则命名 |
| tenantid | 租户（云数据中心）主键 | varchar2\(36\) | 否 | 由平台上下文提供，公有云会使用 |
| sysid | 应用编码 | varchar2\(36\) | 否 | 平台上下文会提供数据 |
| orgid | 工厂 | varchar2\(36\) | 否 | 如果为组织级存组织pk，如果为集团级存集团pk |
| ts | 时间戳 | TIMESTAMP\(6\) | 否 | 每次操作均更新 |
| dr | 删除标记 | varchar2\(36\) | 否 | 默认0 |
| creator | 创建人 | varchar2\(36\) | 否 |  |
| creationtime | 创建时间 | TIMESTAMP\(6\) | 否 |  |
| modifier | 最后修改人 | varchar2\(36\) | 是 |  |
| modifiedtime | 最后修改时间 | TIMESTAMP\(6\) | 是 |  |
| vbillcode | 单据号 | varchar2\(50\) | 是 | 如果定义单据类型则不能为空 |
| approver | 审批人 | varchar2\(36\) | 是 |  |
| approvetime | 审批时间 | TIMESTAMP\(6\) | 是 |  |
| fbillstatus | 单据状态 | int | 否 | 如果节点存在审批流则不能为空 |



