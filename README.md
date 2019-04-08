lin-Choose
===

lin-Choonse描述

三联级滑动选择器

```javascript

  npm install lin-Choose

  import choose from 'lin-choose'
  import 'lin-choose/css/linChoose.css'

  <input type="text" readonly id="inputId" value="1,11,113">

  var chooseObj = new choose();
  chooseObj.init({
        'trigger': '#inputId',
        'keys':{id:'id',name:'name'},
        'data':data
  });

  // 初始显示下标
  chooseObj.value = [0,0,2];

  //data数据格式
  var data = [
    {
        id:1, name:1, child:[
            {
                id:11, name:11, child:[
                    {
                        id:111, name:111
                    },
                    {
                        id:112, name:112
                    },
                    {
                        id:113, name:113
                    },
                ]
            },
            {
                id:12, name:12, child:[
                    {
                        id:121, name:121
                    },
                    {
                        id:122, name:122
                    },
                    {
                        id:123, name:123
                    },
                ]
            }
        ]
    },
    {
        id:2, name:2, child:[
            {
                id:21, name:21, child:[
                    {
                        id:211, name:211
                    },
                    {
                        id:212, name:212
                    },
                    {
                        id:213, name:213
                    },
                ]
            },
            {
                id:22, name:22, child:[
                    {
                        id:221, name:221
                    },
                    {
                        id:222, name:222
                    },
                    {
                        id:223, name:223
                    },
                ]
            }
        ]
    },
    {
        id:3, name:3, child:[
            {
                id:31, name:31, child:[
                    {
                        id:311, name:311
                    },
                    {
                        id:312, name:312
                    },
                    {
                        id:313, name:313
                    },
                ]
            },
            {
                id:32, name:32, child:[
                    {
                        id:321, name:321
                    },
                    {
                        id:322, name:322
                    },
                    {
                        id:323, name:323
                    },
                ]
            }
        ]
    },
  ]

  //此外插件还提供了可直接使用的数据
  import data from 'lin-choose/data/chooseData.js'
  // 地区区域选择数据  keys : {id:id,name:name}
  data.LAreaData


```

![Image text](https://raw.githubusercontent.com/aXin-0810/linChoose/master/img/choose.jpg)


更新日志
=======

  * v1.0.1

许可证
=======

Code copyright 2012-2019 axin_0810
