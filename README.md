# mission-workflow-document
mission system for evaluate work, teamwork use a flowing unit to arrange the work, evalute work effiection, as well as documentation. written by django

# 多人跨部门协作任务系统 
> 工作流梭形流程图系统   

用django写的协同任务系统，用工作流的方式串联各个不同的部门和同事
设计思路，就是用最简单直观的，找人做事的模式：有一个事情（项目），A描述了任务详情，设置了最后期限，之后找到B，告诉B的工作的工作量（B所处节点总值工时以及截止时间），同理B找C，C找D...
另外流程是可以分叉的。每个节点都可以下发多个人来进行。最后组成要给梭形的任务流程图。

另外，还集成了文档系统，通过树来组织文档，可以有多个树。

把评估工作的量，工作绩效加入了此系统。

先看看吧