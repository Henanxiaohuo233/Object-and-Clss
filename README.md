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


