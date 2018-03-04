### sleep()不释放同步锁,wait()释放同步锁,所以sleep()方法没有释放资源,而wait()方法释放了资源
 #### 证据如下:
 ##### The thread releases ownership of this monitor and waits until another thread  notifies threads waiting on this object's monitor to wake up either through  a call to the {@code notify} method or the {@code notifyAll} method.
### sleep(milliseconds)可以用时间制定来使他自动醒过来,如果时间不到你只能调用interreput()来强行打断;wait()可以用notify()直接唤起.
