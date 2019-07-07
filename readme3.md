### 记住我在学习
---
#  ~老子天下第一~
####  **markdown太简单了吧！！！**
>> *markdown*   
![测试](https://ss0.bdstatic.com/94oJfD_bAAcT8t7mm9GUKT-xh_/timg?image&quality=100&size=b4000_4000&sec=1562460512&di=99bb8e82c2cd5e83966c6bab63fb38c6&src=http://b-ssl.duitang.com/uploads/item/201806/28/2018062880919_rrN8V.jpeg)           
## **这是两个主要的学习网站**
  
    
**[百度](http://baidu.com)**          
**[简书](http://jianshu.com)**            
>> 姓名 | 长相 | 排名          
>> -----|-----|------           
>> 王智恒|99.9|2           
>> 郑有为|99.9|3             
>> 张飞|100|1            

**1.hdu1089**       
```   
#include <stdio.h>    
#include <stdlib.h>     
   
int main(void)    
{   
    int a,b;  
    while(scanf("%d%d",&a,&b)!=EOF)     
    {   
           printf("%d\n",a+b);   
    }    
    return 0;   
}   
```      
    
**2.hdu2012**             
###   *Problem Description:*                  
###  **对于表达式n^2+n+41，当n在（x,y）范围内取整数值时（包括x,y）(-39<=x<y<=50)，判定该表达式对于每个给定范围内的取值，如果表达式的值都为素数，则输出“OK”，否则输出“sorry”，每组输入占一行。**             
##  **Input**                   
###  输入数据有多组，每组占一行，由两个整数x，y组成，当x=0,y=0时，表示输入结束，该行不做处理。           
##   **Output**       
###  对于每个给定范围内的取值，如果表达式的值都为素数，则输出“OK”，否则输出“sorry”，每组输入占一行。            
####   Sample Input                
0 1         
0 0     
     
       
####   Sample Output          
ok     
------

##  Source Code:  

```    
#include <stdio.h>    
#include <math.h>   
    
      
int main()   
{   
    int x,y,num,flag,n;    
         
    while(scanf("%d%d",&x,&y)!=EOF)   
    {   
        int t;   
        flag=1;  
           
        for(n=x;n<=y && flag;n++)   
        {   
            t=n*n+n+41;  
               
            for(num=2;num<=sqrt(t);num++)   
        {   
            if((t)%num==0)   
            {  
                flag=0;   
                break;   
            }   
        }   
           
        }   
            if(flag==0)   
                printf("Sorry\n");   
            if(flag &&(x!=0 || y!=0))    
                printf("OK\n");   
           
    }     
       
    return 0;    
}   

```   
   
##    Web sites    
[hdu2012](http://acm.hdu.edu.cn/showproblem.php?pid=2012)     
       
             
