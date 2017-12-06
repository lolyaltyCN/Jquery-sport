# Jquery-sport
this is  jquery Plug-in unit

##一个可扩展jquery的小插件,在当前dom下下落图片或者雪花
options.type = options.type || 2;                   //类型 默认为2  1下图片  2 下雪花
options.direction = options.direction || "down";    //方向 默认为向下
options.num = options.num || 25;                    //数量 默认为向下
options.top = options.top || 0;                     //移动物体的初始top值
options.left =  0;                                  //移动物体的初始left值
options.height = options.height || 0;               //移动物体的高度
options.offset = options.offset || 1;               //移动物体的每次偏移量
options.maxOffset = options.maxOffset || 40;        //移动物体的最大偏移量(差值) 
options.speed = options.speed || 10;                //移动物体的下落速度(毫秒)
options.complete = 0;                               //完成个数
options.before = options.before;                    //开始之前的函数
options.cb = options.cb;                            //完成之后的回调
```
$('.box').sport({
    type:1,
    url:"bir.gif",
    maxOffset:20,
    before:function(){
        console.log('开始之前!');
    },
    cb:function(){
        console.log('全部完成!');
    }
});
```