1. for in 和 for of 的区别
   for in 遍历的是对象(**数组也是对象,不过不推荐**)的键名,for of 遍历的是对象(**可迭代对象**)的键值

2. 什么是可迭代对象
   实现了 Symbol.iterator 方法的对象就是可迭代对象
   Symbol.iterator 方法返回一个迭代器对象,迭代器对象具有 next 方法,每次调用 next 方法都会返回一个对象,对象包含 value 和 done 属性,value 表示当前迭代的值,done 表示是否已经迭代完成 <br>
   常见的迭代器对象有

    1. 数组
    2. 字符串
    3. Set
    4. Map
    5. 类数组对象

    下面就是一个手写的可迭代对象

    ```
    const obj = {
    [Symbol.iterator]: function () {
     let index = 0
     return {
       next: function () {
         if (index < 3) {
           return { value: index++, done: false }
         } else {
           return { value: undefined, done: true }
         }
       }
     }
    }
    }
    ```

3. window.loaded 和 DOMContentLoaded 的区别
   window.loaded 是当**页面所有资源都加载完成后**触发的事件,包括图片,视频,音频等资源
   DOMContentLoaded 是当 DOM 树加载完成后触发的事件,不包括图片,视频,音频等资源
