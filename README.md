# Hello_world
try aut

# -*- coding: utf-8 -*-
public class TrensferProperty {
    int i = 47;                 //成员变量

    public void cali(){         //成员方法
        System.out.println("调用cali方法");
        for (i=0;i<3;i++){      //在方法里调用了成员变量
            System.out.print(i+" ");
        }
        System.out.println();   //换行
    }

    public static void main(String[] args) {
        TrensferProperty t1=new TrensferProperty();//创建两个对象
        TrensferProperty t2=new TrensferProperty();

        t2.i=68;                //改变成员变量的值
        System.out.println("第一次实例变量调用i的结果"+t1.i);//输出成员变量的值
        t1.cali();              //使用成员方法
        System.out.println("第二次实例变量调用i的结果"+t2.i);
        t2.cali();
    }
}

/*  //类
public class Book {
    private String name;                    //定义一个String型的成员变量

    public String getName() {               //定义一个getName()方法
        int id=0;                           //局部变量
        setName("java");                    //调用类中其他方法
        return id+this.name;                //设置方法返回值
    }

    public void setName(String name) {      //定义一个setName()方法
        this.name = name;                   //将参数值赋予类中的成员变量
    }

    public Book getBook(){
        return  this;                       //返回Book类引用
    }

}
*/

/*
局部变量 和 局部变量的有效范围
* */
public class Mytest {
    String name;           //成员变量

    public void getName() {
        int id=0;          //局部变量
        System.out.println(id+name);
    }

    public static void main(String[] args) {
        for (int i=0;i<=10;i++){
            System.out.print("i = "+i);
        }
        System.out.println();
        for (int i=1;i<=10;i++){
            System.out.print("i = "+i);
        }
    }
}


/*
*类的构造方法
*/
public class ClassTest {
    public  ClassTest(){    //一个空参数的构造方法
        // 这个方法也可以不存在，编译器会生成无参数的构造方法
    }

    public static void main(String[] args) {
        ClassTest test=new ClassTest(); //类的对象
    }
}

//分界线 下面是无参数构造方法和有参数构造方法

public class ClassTest {
    public  ClassTest(int a){}  //有参数的构造方法
    public  ClassTest(){};      //无参数的构造方法

    public static void main(String[] args) {
        ClassTest test=new ClassTest(1); //定义参数
        //参数也可以删掉但是要有一个无参数的构造方法
    }
}

//定义无参和有参的构造方法
public class AnyThting {
    public AnyThting(){                     //定义无参构造方法
        this("this 调用有参构造方法");  //使用this调用有参构造方法
    }

    public AnyThting(String name){          //定义有参构造方法
        System.out.println("有参构造方法");
    }

}

//测试
    public class BlackXiao{
        public BlackXiao{}
        Public sest void main(Sting[] args){
            BlackXiao xiao=new BlackXiao(1);
            System.out.println("无参");
        }
    }
    //鸡蛋灌饼
    public class EggCake {
    int eggCount;       //定义对象 初值放在构造方法里面定义
    public EggCake(int eggCount){   //定义有参构造方法
        this.eggCount=eggCount;     //给成员变量赋值
        System.out.println("这个饼里有"+eggCount+"个鸡蛋");
    }

    public EggCake(){               //定义有参
        this(1);           //调用构造方法
    }

    public static void main(String[] args) {
        EggCake e=new EggCake();
        EggCake e2=new EggCake(5);
    }
}

