##Database table names explained 理解数据库表名字

Activiti 的表都以 ACT_ 开头。 第二部分是表示表的用途的两个字母标识。 用途也和服务的 API 对应。

* ACT_RE_*: 'RE'表示 repository。 这个前缀的表包含了流程定义和流程静态资源 （图片，规则，等等）。
* ACT_RU_*: 'RU'表示 runtime。 这些运行时的表，包含流程实例，任务，变量，异步任务，等运行中的数据。 Activiti 只在流程实例执行过程中保存这些数据， 在流程结束时就会删除这些记录。 这样运行时表可以一直很小速度很快。
* ACT_ID_*: 'ID'表示 identity。 这些表包含身份信息，比如用户，组等等。
* ACT_HI_*: 'HI'表示 history。 这些表包含历史数据，比如历史流程实例， 变量，任务等等。
* ACT_GE_*: general 数据， 用于不同场景下。