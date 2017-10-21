# Cg
For storing Java exercises


class	Demo1
{
	public static void main(String[] args) 
	{
		chengJi(64);
		chengJi(73);
		chengJi(25);
		
	}
	/*
	根据考试成绩获取学生分数对应的等级
	90~100		A
	80~89		B
	70~79		C
	60~69		D
	60以下		E
	*/


	public static char chengJi(int a)
	{
		if(a>=90 && a<=100)
			return 'A';
		if(a>=80 && a<=89)
			return 'B';
		if(a>=70 && a<=79)
			return 'C';
		if(a>=60 && a<=69)
			return 'D';
		else
			return 'E';
	}
}
	/*
	首先按照两个明确的方法来写这个函数
	明确一：这个功能的结果是什么？对于这个我的理解是一个char，就是返回值的类型是char
	明确二：这个功能实现的过程中需要的未知内容与运算。这个应该就是学生的分数，是个int
	下面是我重点要说的部分，这是一个未完成的代码。为什么这么说呢，我没有办法检测这个代码的正确性。
	原因是我原计划是把成绩打印到控制台上，可是我不知道在哪个位置写那个语句。
	其实我是有一点思路的，不知道是否可行，就是：
	public static char chengJi(int a)
	{
		if(a>=90 && a<=100)
			System.out.println("A");
		if(a>=80 && a<=89)
			System.out.println("B");
		if(a>=70 && a<=79)
			System.out.println("C");
		if(a>=60 && a<=69)
			System.out.println("D");
		else
			System.out.println("E");
			return;
	}
	这是我思考的结果，可是与我的初衷又有所区别，我希望是在主函数的部分去打印这个东西，可是我并不能实现
	对于我的认知来说，函数应该是一种工具。而我所需要的工具只是判断出分数所对应的字符，并不是直接把成绩打印出来。
	就是说，我想判断分数所对应的成绩，这是我写函数即制作这个所谓的工具的初衷，打印出来只是为了直观的表现。
	我尝试了很多种方式，并不能解决我遇到的问题。所以帮我看一下这个怎么在主函数里写才能打印到控制台上。
	其实我想过，在主函数里面再设一个变量，再写一个打印到控制台的函数。但是这样的话不如再写一个单独的函数，
	用来打印这个东西。可是问题又来了，我输入的是一个int可是函数出来的是个char。搞得我很混乱，所以麻烦帮我看下这个该怎么写很僵硬。
	
	*/
