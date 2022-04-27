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
System.out.println("=========================");
System.out.println("数组概念，定义和数字实现");
//数组的两种形式 不分配内存。
int[] a;//整形数组a。一次可以定义多个数组
int[] a,b,c;整形数组a,b,c;
int a[];//整形数组a。只能一次定义一个数组。

a=new int[10];//形式1
int a1=new a[10];//形式2
System.out.println("=========================");
System.out.println("");
System.out.println("一维数组");
int[] a={1,5,6};
int[] b=new int[3];
b[0]=1;
b[1]=5;
b[2]=6;
System.out.println(a[4]);
//System.out.println(a[3]); //数组溢出
System.out.println("=========================");
System.out.println("");
System.out.println("一维数组赋值输出");
int[] c=new int[10];
for(i=0;i<c.length;i++){
	c[i]=2*i;
	System.out.print(c[i]+"  ");
}
System.out.println("");
for(i=c.length;i>=1;i--){
	if(i==5) System.out.println("");
	System.out.print("数组下标"+(i-1)+"元素值"+c[i-1]+"  ");
	
}
System.out.println("=========================");
System.out.println("");
System.out.println("二维数组赋值输出");

 int[][] aMatrix = new int[4][]; 
    for (i = 0; i < aMatrix.length; i++)  { 
        aMatrix[i] = new int[i+1]; //创建子数组 
        for (int j = 0; j < aMatrix[i].length; j++) { 
          aMatrix[i][j] = i + j; 
        } 
    } 
	
    //输出数组元素 
    for ( i = 0; i < aMatrix.length; i++) { 
      for (int j = 0; j < aMatrix[i].length; j++) { 
        System.out.print(aMatrix[i][j] + " "); 
      } 
      System.out.println(); 
    } 

}
}
