# mission-workflow-document
mission system for evaluate work, teamwork use a flowing unit to arrange the work, evalute work effiection, as well as documentation. written by django

# 多人跨部门协作任务系统 
> 工作流梭形流程图系统   

用django写的协同任务系统，用工作流的方式串联各个不同的部门和同事
设计思路，就是用最简单直观的，找人做事的模式：有一个事情（项目），A描述了任务详情，设置了最后期限，之后找到B，告诉B的工作的工作量（B所处节点总值工时以及截止时间），同理B找C，C找D...
另外流程是可以分叉的。每个节点都可以下发多个人来进行。最后组成要给梭形的任务流程图。

# 一些约定   

- 一个工单的所有流程必须回到发起人手里，此工单才可以被完结！   
- 需要约定固定的审核工单的人（就是能决定事情要不要做的人，**最高决策者**，一般是老板级别的），这是整个系统唯一设置的角色！   
- 工单的发起人可以是任何人，但是第一个流程的审核人是固定的几个人（**最高决策者**）！（为何要这样设置呢：因为为了保证流程的灵活性和不限长度，所以没有设置角色！因为一旦有上下级等角色和权限设定，就破坏了它的灵活性和无限长度的特性！）   
- 必须制定一套制度来确定常规任务的工时数。  
- 除了工单发起人以及最高决策者之外的所有人，都只能把流程转发到同部门的人。   

另外，还集成了文档系统，通过树来组织文档，可以有多个树。

把评估工作的量，工作绩效加入了此系统。

先看看吧

## 流程图样例   

- 根据真实项目截图1，人物名称皆为化名，图片不显示请直接访问 https://www.wendangs.com/img/github/mission-workflow-document/1.jpg      
![真实项目流程截图](https://www.wendangs.com/img/github/mission-workflow-document/1.jpg "真实样例截图")   

- 根据真实项目截图2，人物皆为化名，图片不显示请直接访问 https://www.wendangs.com/img/github/mission-workflow-document/2.png      
![真实项目流程截图](https://www.wendangs.com/img/github/mission-workflow-document/2.png "真实样例截图")   

## 绩效评估   
> 适用于所有的部门！   

图片打不开可以访问https://www.wendangs.com/img/github/mission-workflow-document/3.png   
![真实项目绩效截图](https://www.wendangs.com/img/github/mission-workflow-document/3.png "真实样例截图")   

## 文档界面   
> 树形分类，可以随意移动节点到另一个节点里面/前面/后面，总之就是很方便维护和编辑树   

![真实文档截图](https://www.wendangs.com/img/github/mission-workflow-document/4.png "真实样例截图")   


## TODO
- 搭建展示demo站    
- 开源代码   