 bus
一个事件总线的简单实现
支持多线程
注册事件用方法Bus2.getDefault().register();
主线程订阅方法用
@Subscribe(Bus2.UI_THREAD)
private void funName(){
		
}

工作线程订阅方法用
@Subscribe(Bus2.WORKER_THREAD)

发送线程订阅方法用
@Subscribe(Bus2.POSTING_THREAD)
)
