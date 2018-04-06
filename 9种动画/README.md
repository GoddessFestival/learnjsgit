# learnjsgit
## js原生动画


获得计算后的属性
function getStyle(obj,attr)
 {
  if(obj.currentStyle){
  return obj.currentStyle[attr];
  }
  else{
  return getComputedStyle(obj,false)[attr];
  }
 }

当透明度变化时 兼容IE
 if(attr == 'opacity'){
   obj.style.filter = 'alpha(opacity:'+(icur+speed)+')';
   obj.style.opacity = (icur+speed)/100;
 }


参数fn为回调函数  支持链式动画

 function startMov(obj,json,fn){//fn回调函数

}
