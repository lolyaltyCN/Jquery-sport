# :whale2:Jquery-sport
:whale2:this is  jquery Plug-in unit

##一个可扩展jquery的小插件,在当前dom下飘落图片或者雪花

| options | 默认  | description |
| :------------ |:---------------:| :-----:|
| type          | 2               | 类型 1下图片  2 下雪花 |
| direction     | down            | 方向 |
| num           | 25              |    数量 |
| top           | 0               | 移动物体的初始top值 |
| left          | 0               | 移动物体的初始left值|
| height        | 0               | 移动物体的高度|
| offset        | 1               | 移动物体的每次偏移量|
| maxOffset     | 40              | 移动物体的最大偏移量(差值) |
| speed         | 10              | 移动物体的下落速度(毫秒)|
| before        | null            | 开始之前被触发的函数|
| cb            | null            | 完成之后被触发的回调|

```javascript
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
