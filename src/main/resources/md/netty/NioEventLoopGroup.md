# NioEventLoopGroup
![NioEventLoopGroup](io/NioEventLoopGroup.png)
- NioEventLoop可以认为是个工作线程，scheduledTaskQueue、taskQueue、tailTasks是它的任务池，使用其持有的thread执行任务。NioEventLoopGroup是NioEventLoop的集合，使用EventExecutorChooser策略选择不同的NioEventLoop