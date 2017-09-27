/*abc*/
package simpleCalculators;

import java.util.Random;
/*随机类*/
import java.util.Scanner;
/*导入Scanner类*/
public class szys {
public static void res(){
System.out.println("1.显示结果\t2.直接开始下一题");
}
public static void main (String[] arge){
System.out.println("*****请选择要随机生成的算法*****");
System.out.println("\t1,加法\t2,减法\t3,乘法\t4,除法");
System.out.println("**********");
Scanner sc=new Scanner(System.in 

);
/*将键入的数据赋值给对象sc*/
int s = sc.nextInt();
double result=0;
Random r = new Random();
int a = r.nextInt(100);
int b =r.nextInt(100);
/*将值域设定为0—100*/
switch(s){
case 1:System.out.println("-----|"+a+"+"+b+"=?|-----");result =a+b;res();break;
case 2:System.out.println("-----|"+a+"-"+b+"=?|-----");result =a-b;res();break;
case 3:System.out.println("-----|"+a+"*"+b+"=?|-----");result =a*b;res();break;
case 4:System.out.println("-----|"+a+"/"+b+"=?|-----");{float c=a;float d=b;result=c/d;}res();break;
default:System.out.println("输入有误，重新开始");main(null);break;
}
/*使用switch函数为小学生提供选择*/
Scanner select =new Scanner(System.in 

);
int se =select.nextInt();
switch (se){
case 1:System.out.println("本题的结果："+result);main(null);break;
case 2:main(null);break;
default:System.out.println("输入有误，重新开始");main(null);
}
}
}
