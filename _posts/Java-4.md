layout: post
title: "作业"
data: 2021-8-9 23:13:55 CST
categories: java
* 面向对象程序设计的三个特性？
封装性，多态性，继承性
* 如何用类的成员表示对象的属性和行为的？
Person类值域设计length，year，来表示属性，设计eat方法来表示行为
* 类的成员变量是如何获得初始化的值的？
构造器
* 方法的数据传递有几种，它们各有什么特点？举例说明。
值传递，引用传递，简单类型是值传递，引用类型是引用传递。值传递为不改变原值，引用传递会改变原值。
* 方法重载指什么，创建方法如何才能方法重载？
Person下写public void setYear(int year); 再写public void setYear(double year);就是重载
* 实例成员和类成员有什么不同？
 类成员所有共有，实例成员各个不同
* 创建一个类Point
有成员变量x, y，它们都是int类型。
有四个成员方法setX(int)、setY(int)、getPoint()和movePoint(int,int)。
setX(int)和setY(int)方法是设置成员变量x和y的值；
getPoint()方法则获得由x, y构成的坐标点；
movePoint(int,int)带两个int参数，用来修改x，y构成的坐标点。
```java
public class Point{

    private int x;
    private int y;
    
    public Point(){
        x = 0;
        y = 0;
    }
    
    public void setX(int x){
        this.x = x;
    }
    public void setY(int y){
        this.y = y;
    }
    public void getPoint(){
        System.out.println("("+this.x+","+this.y+")");
    }
    public void movePoint(int x, int y){
        this.x = x;
        this.y = y;
    }
}
```
* Point类有一个构造方法，不带参数，为x, y设置原点值。
另一个类为TestPoint，有一个main()方法，用来对Point类的实例进行测试。要求为其实例设置(0,0)坐标点，再移动到(10, 20)坐标点上，并输出实例调用相应的方法的结果
```java
public class TestPoint{
    public static void main(String[] args){
        Point point_test = new Pointer();
        point_test.setX(0);
        point_test.getPoint();
        point_test.setY(0);
        point_test.getPoint();
        point_test.movePoint(10,20);
        point_test.getPoint();
    }
}

```

![capture_20210915222636457](D:\SoftwareData\Nutstore\Cloud\我的坚果云\1_Work\material\capture_20210915222636457.bmp)
