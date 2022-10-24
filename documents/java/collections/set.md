> Set集合中不能保存重复的元素，并且最多允许有一个null元素

Set 实现了Collection类， 它主要有两个常用的实现类： `HashSet`和`TreeSet`

### HashSet

HashSet 内部使用了HashMap存储数据，将数据存入了HashMap 的key中，所有数据是不能重复的，根据数据的hashcode和equals方法判断是否重复。

### TreeSet

TreeSet 同时还实现了 SortedSet接口，所以TreeSet中的数据默认情况下是自然排序的，这里的自然排序指的是升序排序。

TreeSet 只能对实现了 Comparable 接口的类对象进行排序。
