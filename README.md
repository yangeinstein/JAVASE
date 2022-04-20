# JAVASE
## 第二章
import java.util.Random;
class WhileDemo{
public static void main(String args[]) {
int i;     //初始化条件
int sum=0;
/* for(int j=0;;j++){
	for(i=0;;i++)
	{
		System.out.print("第"+i+"次数"+"Welcom to Java!  ");

	}
	System.out.println("j为第"+j);
}
/*for(i=0;;i++){
	System.out.print("第"+i+"次数"+"Welcom to Java!  ");
}*/
System.out.println("长方形输出");
for(int j=0;j<=4;j++){
	for(i=0;i<=19;i++)
	{
		System.out.print("*");

	}
	System.out.println();
}


for(i=1;i<=5;i++){
	if(i==2){
		System.out.println("第"+i+"次单次循环结束，继续后续循环");
		continue;
		}
	if(i==4){
		System.out.println("第"+i+"次整体循环结束，后续不循环");
		break;
	}
	System.out.println("第"+i+"次");
}
System.out.println("整个程序结束");
System.out.println("=========================");
System.out.println("三角形输出");
for(int j=0;j<=9;j++){
	if(j==6){
		continue;
	}
	for(i=0;i<=j;i++)
	{
		System.out.print("*");
     
	}
	System.out.println(j);
	
	if(j==8){
		break;
	}
}
System.out.println("ppt案例BreakLoop2");
for(int j=0;j<3;j++){
	System.out.print("pass"+j+":");
	for(i=0;i<100;i++)
	{
		if(i==19){break;}
		System.out.print(i+" ");
     
	}
	System.out.println();
}
System.out.println("整体循环结束");

System.out.println("=========================");
boolean t = true;
one: {
      two: {
         three: {
                 System.out.println("three程序块中break之前的输出.");
                    if(t) break three;                // 跳出two程序块的语句
                   System.out.println("three程序块中break之后的输出.此句将不被执行");
                   } 
            System.out.println("two程序块中的输出.此句将不被执行");
           }
 System.out.println("one程序块中的输出.此句不受影响，照常输出.");
    }
System.out.println("输出20～100之间不能被7整除的整数不用continue");
System.out.println("=========================");
	for(i=20;i<=100;i++){
		if(i%7!=0){
		System.out.print(" "+i);
		}
	}
    
System.out.println("输出20～100之间不能被7整除的整数用continue");
System.out.println("=========================");
for(i=20;i<=100;i++){
		if(i%10==0)
		System.out.println(" ");
		if(i%7==0) continue;
		else
	    System.out.print(" "+i+" ");
	}
    
System.out.println("=========================");	
System.out.println("50~100显示能被7整除并能被8整除的数");
for(i=50;i<=100;i++){
if(i%7==0){
	if(i%8==0){
		System.out.print(" "+i+" ");
	}
}
	if((i%7==0)&&(i%8==0))
		System.out.print(" "+i+" ");
}

System.out.println("=========================");
System.out.println("50~100显示能被7整除或者能被8整除的数");
for(i=50;i<=100;i++){
//	if((i%7==0)||(i%8==0))
//	System.out.print(" "+i+" ");
if(i%7==0){System.out.print(" "+i+" ");}
if(i%8==0){System.out.print(" "+i+" ");}
}
System.out.println();

System.out.println("=========================");
System.out.println("50~100显示能被7整除或者能被8整除的数  有问题代码");
for(i=50;i<=100;i++){
	if(i%7!=0){
		continue;
	}else
	    System.out.print(" "+i+" ");
	if(i%8!=0){
		continue;
	}else
System.out.print(" "+i+" ");}

System.out.println("=========================");
System.out.println("50~100显示能被7整除和能被8整除的数");
for(i=50;i<=100;i++){
	if((i%7!=0)||(i%8!=0)) continue;
	else
	System.out.print(" "+i+" ");	
 }
 System.out.println();
 
 System.out.println("=========================");
System.out.println("九九乘法口解表");
out:for(i=1;i<=9;i++)
	{
	for(int j=1;j<=9;j++)
	{ 
		if(j>i){System.out.println("");continue out;}
		if(j*i<=9){
			 System.out.print(" ");
		}
		System.out.print(j+"X"+i+"="+(j*i)+" ");
	}
}
 System.out.println();
 System.out.println("=========================");
System.out.println("阶乘");
sum=1;
for(i=1;i<=10;i++){
	sum*=i;
System.out.println(sum);
}
System.out.println("=========================");
System.out.println("**while 语句**"); 
sum=1;
i=1;
while(i<=10){
	sum*=i;
	i++;
	System.out.println(sum);
}
System.out.println("=========================");
System.out.println("50个随机整数");

for(i=1;i<=50;i++){
	Random r = new Random();
	sum = r.nextInt(100);
	System.out.print(" "+sum);
	if(sum%5==0)
	//System.out.println("");
	System.out.println("被5整除"+sum);
	}

}
}
