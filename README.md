# create-
面向对象之创建方式
三种方式创建面向对象
  1，通过new关键字来创建
      var add = new add()
  2，通过字面量来创建
    2.1 简单字面量
      var obj = {};
      obj.name ="ben"
      obj.todo = function(){
            return this.name
        }
      2.2嵌套字面量
      var obj = {
        name:'ben',
        age:29,
        todo:function(){
          console.log(this.name)
        }
      }
     2.3函数声明与函数表达式
     function add(){}
     var add1 = function(){}
  3,构造函数
  function Person(name,age){
    this.name = name;
    this.age = age;
    this.todo = function(){
        return this.name
     }
  }
  var person = new Person('ada',12)
  console.log(person.name)
  
  二 funtion person(name){
            return name
  }
  person('add');
      1.工厂模式
             function Person(name,age){
                    var obj = new Object();             
                    this.name = name;
                    this.age = age;
                    return obj
                 }
  
               var a1 = Person('aa',33)
                   a1.name
                   
        2.构造函数与普通函数的区别
         this指向
            构造函数的this指向创建的对象实例上
            普通函数的函数调用者
         调用方式
           构造函数 NEW
          命名方式
          构造函数首字母大写
            
  
  //案列
  var obj = {
  	init:function(){
	        this.bind();
            this.popup();
	},
	bind:function(){
            $(".nstent .list-b").hover(function(){
                $(this).find(".see").show();
            }.function(){
                $(this).find(".see").hide();
            }
        })
        $("#see").click(function(){
                $(".bg .popupbox").show();
        })        
        $(".btn3  .cancel).click(function){
                $(".bg .popupbox").hide();
        })
   },
    popup:function(){
     var box = $('.nstent');
     var _width = document.body.clientWidht;
     var _hight = document.body.clientHeight;
     var $width = (_width - box.width())/ 2;
     var $hight = (_hight - box.height())/ 2;
     popupbox.css({'width':$width,'height':$hight})
   }
  }
  
  
  $(function(){
        obj.init();
  })
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
