# Hello_world
try aut

# -*- coding: utf-8 -*-
import requests
import java.awt.*;
import java.util.Date;
import java.util.Scanner;


public class Link {
        public static void main(String[] args) {
            /*
             String str = "Wa are students";   //定义字符串str
             int size = str.indexOf("a");      //将字符串str赋值给size
             System.out.println(size);         //输出a在str里面的首次出现位置
             */

            /*
            String str ="We are students";
            //将空格字符串在str中的索引位置赋值给变量size
            int size = str.lastIndexOf("");
            //将变量size输出
            System.out.println("空格符在字符串str的索引位置是："+size);
            //将字符串str的长度输出
            System.out.println("字符串str的长度是："+str.length());

             */
            /*
            String str2="hello word";    //定义字符串str
            char mychar = str2.charAt(5);//将字符串索引位置是6的字符返回
            System.out.println(mychar); //输出信息

             */
            /*      截取字符串   substring
            String str="Hello wold";            //定义字符
            String substr = str.substring(3);   //对字符串进行截取
            System.out.println(substr);         //输出截取后的字符串
                                                //输出值为lo Word
             */
            /*
            String str = "Hello Wold";          //定义字符
            String substr = str.substring(3,7); //对字符串进行截取 中间用逗号隔开
            System.out.println(substr);         //输出结果为Hel
             */
            /*      去除空格 用法 trim
            String str = "   Java  class   ";                   //定义字符
            System.out.println("原来字符串的长度"+str.length());   //将str的原有长度输出
            //将 str 去掉前导和尾部的空格后的结果输出
            System.out.println("修剪后的长度"+str.trim().length());
            //输出结果为：
            //原来字符串的长度17
            //修剪后的长度11
             */

             /* // 替换字符 replace
            String str="address";                                   //定义字符
            //将字符串str中的字符”a“替换成”A“后返回的新字符串 newstr
            String newstr = str.replace("a","A");
            System.out.println(newstr);                             //输出结果为Address
             String str = "java proeject"; //定义字符
            //将str字符 里面小写 j 全部替换为大写 J
             String newstr = str.replace("j","J");
             //输出结果 Java proeJect
             System.out.println(newstr);
             //错误示范
             String str2 = "java proeject";
             String towstr = str.replace("P","t");
             System.out.println(towstr);//输出结果为java ptoeject 没有改变
              */
             /*
                //判断字符串的开始于结尾   判断前缀是 startsWith(),判断后缀是 endsWith()
            String num1="6678451899";           //定义字符num1
            String num2="9541234169";           //定义字符num2
            boolean b = num1.startsWith("66");  //判断字符串num1是否以 66 开头
            boolean b2= num1.endsWith("98");    //判断字符串num1是否以 98 结尾
            boolean b3= num2.startsWith("96");  //判断字符串num2是否以 96 开头
            boolean b4= num2.endsWith("69");    //判断字符串num2是否以 69 结尾
            System.out.println("字符串num1开始以'66'开始的吗"+b);  // 字符串num1开始以'66'开始的吗true
            System.out.println("字符串num1是一'98'结束的吗"+b2);   //字符串num1是一'98'结束的吗false
            System.out.println("字符串num2开始以'96'开始的吗"+b3); //字符串num2开始以'96'开始的吗false
            System.out.println("字符串num2是一'69'结束的吗"+b4);   //字符串num2是一'69'结束的吗true
            //输出结果为
              */
             /*
                //判断字符串是否相等 分大小写判断用equals() 或 不分大小写判断用 equalsIgnorCase()
            String s1 = new String("abc");  //创建字符串对象
            String s2 = new String("ABC");
            String s3 = new String("abc");
            boolean b = s1.equals(s2);              //使用 equals()方法比较s1与s2
            boolean b2= s1.equalsIgnoreCase(s2);    //使用equalsIgnoreCase比较s1与s2
            System.out.println(s1+"equals"+s2+":"+b);
            //输出结果：abcequalsABC:false
            System.out.println(s1+"equalsIgnoreCase"+s2+":"+b2);
            //输出结果：abcequalsIgnoreCaseABC:true
              */
                /*
             //按字典顺序比较两个字符串     compareTo
             String str = new String("b");
             String str2= new String("a");      //用于比较的三个字符串
             String str3= new String("c");
             System.out.println(str+" compareTo"+str2+":"+str.compareTo(str2));
             //将 str 于 str2比较的结果输出
             System.out.println(str+" compareTo"+str3+":"+str.compareTo(str3));
             //将 str 于 str3比较的结果输出
               // d compareToa:1       输出结果
               // d compareToc:-1        输出结果
                 */

                /*字符串转换大小写      转小写是toLowerCase   转大写是toUpperCase
            String str = new String("abc DEF"); //创建字符
            String newstr = str.toLowerCase();   //使用 toLowerCase()方法实行小写转换
            String newstr2 = str.toUpperCase();  //使用 toUpperCase()方法实行大写转换
            System.out.println(newstr);          //输出结果：abc def
            System.out.println(newstr2);         //输出结果：ABC DEF
                 */
                /*
                字符串分割 两种分割方法一种 str.split(根据分隔符分割)
                可以定义别的分隔符用反斜杠(\\ )进行转意
                第二种是在str.solit(分隔符,数字)
            String str = "abc,def,ghi"; //定义字符
            String[] strArray = str.split(","); //对str进行分割
            for (String tmp:strArray){                //进行循环输出str
                    System.out.print("["+tmp+"]");
            }
                System.out.println();

            String ip="168.162.0.1";
            //创建字符串
            String[] fistArray = ip.split("\\.");
            //按照“.”进行分割，使用转义字符“\\.”
            String[] tuoArray = ip.split("\\.",2);
            //按照“.”进行两次分割，使用转义字符“\\.”
            for (String tmp:fistArray){
                    System.out.print("["+tmp+"]");
            }
            //输出全部分割的结果
            System.out.println();
            //换行
            for (String tmp:tuoArray){
                    System.out.print("["+tmp+"]");
            }
            //输出层分割两次的结果
            //输出结果    [168][162][0][1]
            //输出结果    [168][162.0.1]
                 */

                /* 日期和时间字符串格式化 format
            Date date = new Date();               //创建 Date 对象 date
            String s = String.format("%te",date); //通过 format()方法对 date进行格式化
            System.out.print(s);                  //输出结果为 24
                 */

                /*
                Date date = new Date();
                //创建 Date 对象 date
                String year = String.format("%tY",date);
                //将 date 格式化
                String month = String.format("%tB",date);
                String day = String.format("%td",date);
                System.out.print("今年是："+year+"年");
                //输出信息
                System.out.print("现在是："+month);
                System.out.print("今天是："+day+"号");
                 */
                /*
                Date date = new Date();//创建Date 对象 date
                String hour = String.format("%tH",date);//对date进行格式化
                String minute = String.format("%tM",date);
                String second = String.format("%tS",date);
                String weim = String.format("%tp",date);
                System.out.println("现在是："+weim+hour+"时"+minute+"分"+second+"秒");
                //现在是：20时52分29秒

                 */
                /*
                Date date = new Date(); //创建 Date 对象 date
                String time = String.format("%tc",date);
                //对date进行时间组合格式化
                String form = String.format("%tF",date);
                System.out.println("全部的时间信息是："+time);
                //输出信息
                System.out.println("年-月-日的格式是："+form);

                 */
                /*常规类型格式化
                String str = String.format("%d",400/2); //将结果以十进制格式显示
                String str2 = String.format("%b",3>5);  //将结果以boolean型显示
                String str3 = String.format("%x",200);  //将结果以十六进制格式显示
                System.out.println("400的一半是多少："+str);//输出结果：400的一半是多少：200
                System.out.println("3>5正确吗？："+str2);   //输出结果：3>5正确吗？：false
                System.out.println("200的16进制数是："+str3); //输出结果：200的16进制数是：c8

                 */
                //使用正则表达式
                /*
                String regex = "\\w+@\\w+(\\.\\w{2,3})*\\.\\w(2,3)";
                String a = "aaa@";
                String a2 = "aaaaaa";
                String a3 = "1111@163.vip.com";
                String a4 = "outman@163.com";
                if (a.matches(regex)) {
                        System.out.println("a  这是个合法的邮箱");
                }
                if (a2.matches(regex)) {
                        System.out.println("a2 这是个合法的邮箱");
                }
                if (a3.matches(regex)) {
                        System.out.println("a3 这是个合法的邮箱");
                }
                if (a4.matches(regex)){
                        System.out.println("a4是一个合法字符");
                }

                 */
                /*
                Scanner sc=new Scanner(System.in);
                String regex = "(13[0-9]|15[012356789]|18[056789])\\d{8}";
                while (true){
                        String phone = sc.nextLine();
                        if (phone.matches(regex)){
                                System.out.println("您输入的是手机号");
                        }else{
                                System.out.println("您输入的不是手机号");
                        }
                }

                 */
                //字符串生成器
                /*
                String str = "";
                long starTime = System.currentTimeMillis();
                for (int i = 0;i<10000;i++){
                        str = str + i;
                }
                long endTime = System.currentTimeMillis();
                long time = endTime - starTime;
                System.out.println("Sting 消耗时间："+time);
                StringBuffer builder =new StringBuffer();
                starTime = System.currentTimeMillis();
                for (int j =0;j<10000;j++){
                        builder.append(j);
                }
                endTime = System.currentTimeMillis();
                time = endTime - starTime;
                System.out.println("StringBuilder 消耗时间："+time);

                 */
                /*
                //追加字符序列 append();
                StringBuffer sbf = new StringBuffer("门前大桥下,");
                sbf.append("游过一群鸭,");
                StringBuffer tmp = new StringBuffer("快来快来数一数");
                sbf.append(tmp);
                int x = 24678;
                sbf.append(x);
                StringBuffer mmp = new StringBuffer("我在加一个看看");
                sbf.append(mmp);
                System.out.println(sbf);
                 */
                StringBuffer sbf = new StringBuffer("0123456");
                //创建StringBuffer类 sbf
                sbf.setCharAt(3,'A');
                //索引位置3 更换为 A
                System.out.println(sbf);
                //输出结果：012A456
                StringBuffer sbf2 = new StringBuffer( "0123456");
                //创建sbf2
                sbf2.insert(3,'插');
                //索引 3位置插入 插
                System.out.println(sbf2);
                //输出结果：012插3456789
                StringBuffer sbf3 = new StringBuffer("我爱你，你爱他");
                //创建字符 sbf3
                sbf3 = sbf3.reverse();
                //将字符序列sbf3 翻转 赋值给sbf3
                System.out.println(sbf3);
                //输出结果：他爱你，你爱我

                StringBuffer sbf4 = new StringBuffer("天行健，君子以自强不息");
                //创建字符 sbf4
                sbf4 = sbf4.delete(4,7);
                //指定索引位置删除
                System.out.println(sbf4);
                //输出结果：天行健，自强不息
                
                StringBuffer sbf = new StringBuffer("故事春晓");//定义字符
                sbf = sbf.delete(0,2);                         //删除索引位置:故事
                sbf = sbf.insert(1,"眠不觉");          //在索引1的位置插入:眠不觉
                sbf.append(",处处闻啼鸟");                       //追加字符
                System.out.println(sbf);                 //输出结果:春眠不觉晓,处处闻啼鸟
                //--------------------------------------------------------------
                章后小结
                //大小写转换
                String str = new String("ABCdef");
                String str2 = str.toUpperCase();
                String str3 = str.toLowerCase();
                System.out.println(str2);
                System.out.println(str3);
                
                //str追加0-10
                StringBuffer ste = new StringBuffer("str"); //实例化StringBuffer对象
                for(int i=0;i<=10,i++){
                        str.append(i);                      //通过for循环向Str追加1~10
                }
                System.out.println(str);                    //输出结果为str012345678910
                
                //大陆手机号判断
                Scanner sc =new Scanner(System.in);
                String regx = "(13[0-9]|15[012356789]|18[056789])\\d{8}";
                while (true){
                        String phone= sc.nextLine();
                        if (phone.matches(regx)){
                                System.out.println("是手机号");
                        }else{
                                System.out.println("不是手机号");
                        }
                }
                //截取字符串后比较 比较字符串的时候不能使用== = 要使用equal或                                                                           equalsIgnoreCase
                String str="Hello,java";
                String str1="1Hello,java";
                String substr = str.substring(0,4);
                String substr1= str1.substring(0,4);
                if (substr.equalsIgnoreCase(substr1)){
                        System.out.println("两个字符串相等");
                }else{
                        System.out.println("两个字符串不相等");
                }
                
        }
}

