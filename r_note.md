c(1,2,3,4) refers to a long vector
#  refers to comment
array in r is started with index 1
b=c(1,2,3,4,5,6,7)
b[7] is 7
b[1:6] is c(1,2,3,4,5,6)
in square brackets are fiter condition to fetch elements of the vector.
	class(x) : 查看对象的类型 to determine the class of an object.
summary(lm(dist~speed,data=cars))

data()  获取数据
ls() 查看工作空间中的变量
names() 查看名字
#graph
hist 直方图
stripchart 随机散点图
plot() 二维散点图
dotplot(Amount~Year|food, comsuption) 二维散点图
在一个函数中，如果一个包不存在，执行到library将会停止执行，require则会继续执行。require将会根据包的存在与否返回true或者false，
Objects Are Copied in Assignment Statements
This is also true in function calls.
