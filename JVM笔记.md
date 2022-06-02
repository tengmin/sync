-Xms和-Xmx
（1）-Xms 为JVM启动时申请的初始Heap值，默认为操作系统物理内存的1/64但小于1G。默认当空余堆内存大于70%时，JVM会减小heap的大小到-Xms指定的大小，可通过-XX:MaxHeapFreeRation来指定这个比列。
（2）-Xmx 为JVM运行时可申请的最大Heap值，默认值为物理内存的1/4但小于1G，默认当空余堆内存小于40%时，JVM会增大Heap到-Xmx指定的大小，可通过-XX:MinHeapFreeRation来指定这个比列。

-XX：MaxPermSize