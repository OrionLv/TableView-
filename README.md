# TableView-
TabView二级列表的一个小demo

###这里讲下实现的原理：
1. 首先有个控制seciton展开和关闭的数组sectionStatus，里面的元素是由0和1组成，初始化的时候，全部是0
2. 利用tableView的HeadView 创建的时候 我在headView的代理方法中返回的是一个button,然后把section绑定为button的tag
3. 在button的点击事件中，点击的时候，sectionStatus中的对应tag值的那个元素 用1替换掉 然后刷新对应的section
4. 返回每组section的个数的时候，根据sectionStatus数组中的0和1进行返回
####下面是图片：
![demo.gif](http://upload-images.jianshu.io/upload_images/2477606-5aaa7f8b695d829d.gif?imageMogr2/auto-orient/strip)
