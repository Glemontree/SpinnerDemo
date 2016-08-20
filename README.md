# SpinnerDemo
This demo is to show how to use spinner , and the codes refers to the codes created by zhangyayun.
根据案例总结如下：
1.在values目录下新建一个xml文件，并且在定义数据内容时，使用<string-array>元素指定，要注意<string-array>标签应当放在<resouces>标签下，对于所有的资源，都应当放在<resources>标签下；
2.在使用<string-array>定义数据内容时，通过name指定string-array的名字，这样在程序中可以通过R.array.name来获取
3.android:entries="@array/book"
		这个格式是规定的 @后面不是文件名。
		因为这是android里面的约定 资源文件里面的数组都用R.array.xxx表示
		就如同要找到组件布局必须用R.layout.xxx表示一样
		book是数组名 存在values下
		声明：
 		<string-array name="book" >
        	<item >1</item>
        	<item >2</item>
        	<item >3</item>
        	<item >3</item>
		</string-array> 
4.String[] cities = getResources().getStringArray(R.array.city_labels);//获取资源数据的方法
5.提示信息的设置：spinnerCountry.setPrompt("选择国籍：");// 在列表中显示
6.此外可以用adapter.setDropDownViewResource(android.R.layout.simple_spinner_dropdown_item);//来设置显示风格
