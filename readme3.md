### 记住我在学习
---
#  ~老子天下第一~
####  **markdown太简单了吧！！！**
>> *markdown*   
![timg](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1562310523202&di=e440ba0a9607e47b11ceb7055ed6adaa&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120211%2F7447807_175725670000_2.jpg"小猫")        
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
OK   
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
       
             
