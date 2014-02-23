### What's Integrate

Integrate有整合和集成的涵义，这个项目的核心目标是让团队的每个成员的想法产生交流和融合，
特别是对于远程协作的团队，如何敏捷起来，这将是一个值得努力的尝试。

### The Model：数据模型

1. Scene场景

    {
        "name":场景的名称,如：登录，注册
    }

    关系：Scene拥有很多的View

2. View视图

    {
        "description":描述
        "path":图片的存储地址
    }

    关系：View属于某一个Scene，同时View拥有很多的Talk

3. Talk讨论
    {
        "topic":讨论的主题
		"host":讨论发起人
		"state":讨论状态，关闭，进行
		"conclusion":讨论结论
    }

    关系：Talk属于一个View，同时Talk拥有很多的Speak

4. Speaking留言

    {
        "spokenman":发言人名字,
        "content": 内容
    }

    关系：Speaking属于一个Talk

### 业务逻辑

Scene

1. 创建Scene:

    scene/create

2. 展现Scene：

    scene/list

3. 删除Scene

    scene/del

4. 编辑Scene

    scene/edit

View

1. 创建View:

    view/create

2. 展现View：

    view/list

3. 删除View

    view/del

4. 编辑View

    view/edit

Talk

1. 创建Talk:

    talk/create

2. 展现Talk：

    talk/list

3. 关闭Talk

    talk/close

4. 重开Talk

    talk/reopen

Speaking

1. 创建Speaking:

    speaking/create

2. 展现Speaking：

    speaking/list


