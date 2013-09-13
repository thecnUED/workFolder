# 机试考查

题目开放，请自由作答。

## HTML

* 要求：用html描诉设计图（不需要完成样式，请添加必要的结构性class）
* 提示：html语义化，W3C 标准应用

![html test](https://coursenetworking.atlassian.net/secure/attachment/16115/gradebook-item.png)

## CSS

请写一个全站通用按钮组件

* 要求：简单易用，不需要特别完备，实现思路即可。（兼容IE8+）
* 提示：可参考[Bootstrap - Button groups](http://getbootstrap.com/2.3.2/components.html#buttonGroups)的实现

## Javascript

1. 说明下面代码的运行结果和做简单的说明。

    ```javascript
    var name = 'alvin';
    function echo(){
        alert(name);
        var name = 'elson';
        alert(name);
        alert(age);
    }
    echo();
    ```

2. 使用原生Javascript实现下面代码：点击li后alert出当前的index值

    ```html
    <ul id="target">
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
    </ul>
    ```

3. 用javascript实现一个简单的数据模型

```javascript
    //创建一个Model对象，需要实现的功能：
    var Asset = Model.create();
    var asset = Asset.init();
    var asset2 = Asset.init();

    asset.name ='alvin';
    console.log(Asset.find(asset.id).name);//undefined
    asset.save();
    console.log(Asset.find(asset.id).name);//alvin

    asset2.name = 'elson';
    asset2.save();
    console.log(Asset.find(asset.id).name);//elson

    var Person = Model.create();
    console.log(Person.find(asset.id).name);//undefined
```
