> List 接口继承了Collection接口，拥有Collection的全部方法，同时也有一些自己专用方法。

  常用方法

| 方法名                                      | 描述                                                         |
| ------------------------------------------- | ------------------------------------------------------------ |
| addAll(int index, Collection c): boolean    | 在当前list的指定位置插入集合的全部元素，返回boolean类型      |
| get(int index): E                           | 从集合的指定位置获取元素                                     |
| set(int index, E element): E                | 以指定元素替换list指定位置的元素，返回被替换的元素           |
| add(int index, E element): void             | 在此列表的指定位置插入指定元素，将当前位于该位置的元素和后续元素向后移动（将其索引加一） |
| remove(int index): E                        | 移除此列表的指定元素。将任何后续元素向左移动（将其索引减一），返回从列表中删除的元素 |
| indexOf(Object o): int                      | 返回列表中指定元素第一次出现的索引，如果列表不包含该元素，则返回-1 |
| lastIndexOf(Object o): int                  | 返回列表中指定元素最后一次出现的索引，如果列表不包含该元素，则返回-1 |
| listIterator(): ListIterator                | 返回一个list中元素的迭代器                                   |
| listIterator(int index): ListIterator       | 返回一个从list中指定索引开始的元素迭代器                     |
| subList(int fromIndex, int toIndex): List   | 返回一个子列表，子列表不可变                                 |
| replaceAll(UnaryOperator<E> operator): void | 把list中的所有元素通过运算替换为新的元素                     |
| sort(Comparator<? super E> c): void         | 使用指定的比较器对该列表进行排序                             |

List中存储的数据是有序的，可重复的。常用的实现类有`ArrayList` 和 `LinkedList`

### ArrayList

使用数组实现的List，内部使用数组保存数据，支持动态扩容。特点是查找操作快，

### LinkedList

使用链表实现的List



