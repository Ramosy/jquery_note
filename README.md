# jquery_note
## jquery笔记

### 1.jQuery.extend()
#### 功能一:追加jQuery对象的添加静态方法
##### 举个栗子:
    jQuery.extend({
	    test:function(){
	    console.log("测试jQuery.extend");
	    }
    });
    $.test()
##### 功能二:扩展的对象,常用来合并对象
    var A = { one: false, two: 5, three: "foo" }; 
    var B = { one: true, two: "bar" }; 
    jQuery.extend(A, B); 
    结果:
	A 是 { one: true, two: "bar", three: "foo" }
    B 是 { one: true, two: "bar" }不变  
    