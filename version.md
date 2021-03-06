## 发布工程师制定发布计划

* 发布工程师在JIRA的版本管理中增加下一步发布版本的时间与主版本号
* 次要的集成序号暂时不填，默认为BuildNext
* 版本的名称规范如下:产品名-主版本号-集成编号,如(UMP-R2.0-Build117485,RDS_R3.5_Build119821等).

## 测试工程师测试已发布版本

* 对于发现的BUG或改进项目，及时的进行上报
* 在上报的BUG或改进项目中，选择当前的测试版本为受影响的版本(能否进行多选？)表示该bug影响多个版本

## 开发工程师修复BUG

* 开发工程师在修复BUG时要选择修复的版本为下一个版本(即尚无build号的版本)

## 开发工程师完成任务或功能(Task)

* 开发任务可以由开发工程师和项目经理创建Task类型的缺陷。
* 发布Task时，受影响的版本应该是最近的已发布版本，这样以后就能知道这个任务或功能是哪个版本中被引入的。
* 完成Task时，修复版本也选择下一个版本(即尚无build号的版本)

## 集成工程师集成与发布

* 集成工程师进行集成获得最新的Build号，修改到BuildNext版本中。
* 集成工程师要将版本管理中的版本状态修改为已发布

## 测试工程师验证与关闭

* 测试工程在新版本发布后，需要对发布版本的修改的BUG和完成改进进行验证
* 验证通过则关闭BUG
* 验证不通过，需要将影响版本修改为当前测试版本，并且将修正版本修改为未知。



## 发布工程师归档版本

* 如果已发布的旧版本已经不再维护，可以将该版本状态修改为归档状态。





