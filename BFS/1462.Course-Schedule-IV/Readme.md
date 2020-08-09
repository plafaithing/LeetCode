### 1462.Course-Schedule-IV

考虑到n<=100，即使将每个节点的所有先修课程都记录下来，时间复杂度o(n^2)也是可以接受的。于是本题就是常规的拓扑排序算法，需要特别处理的是：每次从cur拓展到下一个next节点时，要把cur的所有先修课程都复制一遍给next。至于数据结构，显然用集合来实现去重和查询query都很方便。