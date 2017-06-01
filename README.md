# jquery_note
### 1.jQuery.extend()
#### 功能一:追加jQuery对象的添加静态方法[拓展个全局函数]
##### 举个栗子:
    jQuery.extend({
	    test:function(){
	    console.log("测试jQuery.extend");
	    }
    });
    $.test()的输出是测试jQuery.extend
##### 功能二:扩展对象,常用来合并对象
    var A = { one: false, two: 5, three: "foo" }; 
    var B = { one: true, two: "bar" }; 
    jQuery.extend(A, B); 
    结果:
	A 是 { one: true, two: "bar", three: "foo" }
    B 是 { one: true, two: "bar" }不变  
### 2.jQuery.fn.extend()
#### 功能:拓展实例化的jQuery对象的方法
	 jQuery.fn.extend({
	    test:function(){
	    	console.log($(this).height())
	    }
    });
    $("body").test()输出的body的高度
### 总结：jQuery.extend和jQuery.fn.extend的区别在于前者处理jQuery对象，后者是处理jQuery实例对象

    