一个草原上有500只老虎，一只羊，
老虎和羊都可以吃草生活，就会变成羊，

1. 不吃 吃了之后会变成羊 
   如果只有一只老虎，就会吃羊
2. 吃，羊肉好吃，
   有两只老虎，一只羊  不吃
3. 不吃， 羊羊那么可爱   做个朋友吧
   三只老虎，一只羊   吃，
   四只老虎，不吃  
   五只老虎   吃

   大事情难解决，分成小事情，
   大事化小，   递归  
   fn = !(fn-1)
   边界 n = 1 吃，n = 2 不吃
   500只老虎，不吃

    动态规划（Dynamic Programing）是常考算法，上楼梯问题
    三个术语：1. 最优子结构  500-》499-》。。。。。2-》1
             2. 边界 n = 1 吃，n = 2 不吃
             3. 状态转移公式  虎变羊 f(n) = !(fn-1)

    
    楼梯台阶有12阶，一步只能走1阶或2阶，请问有多少种走法
    最优子结构  f(12)
      f(12)   f(11) f(10)
    边界  1  台阶 1  
          2  台阶 2
    状态转移公式  f(12) = f(11) + f(10)



   