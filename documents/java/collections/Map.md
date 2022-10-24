> Map 是一种 key，value 结构的数据，map中存放的key不允许重复

常用方法

| 方法名称                       | 说明                                                         |
| :----------------------------- | ------------------------------------------------------------ |
| size()                         | 返回map中的元素个数                                          |
| isEmpty(): boolean             | 是否是空的map                                                |
| containsKey(object): boolean   | 是否包含key（object）                                        |
| containsValue(object): boolean | 是否包含value（object）                                      |
| get(object): V                 | 获取key对应的value                                           |
| put(k, v): V                   | 往map中放入一组数据，返回的是key对应的前一个值，如果没有则返回null |
| remove(object): v              | 移除key对应的数据                                            |
| keySet(): Set<k>               | 返回key值对应的集合                                          |
| values(): Collection<v>        | 返回value值对应的集合                                        |
| entrySet(): Set<Entry<K, V>>   | 返回map数据转为set后的集合                                   |
| clear(): void                  | 清空map                                                      |

遍历Map的方法

```java
// Map遍历的方法
Map<String, Object> map = new HashMap<>();
map.forEach((k, v) -> {
    System.out.println("key:" + k);
    System.out.println("value:" + v);
});

map.keySet().forEach(k -> {
    System.out.println("key:" + k);
    System.out.println("value:" + map.get(k));
});

for (Map.Entry<String, Object> entry : map.entrySet()) {
    System.out.println("key" + entry.getKey());
    System.out.println("value" + entry.getValue());
}

Iterator<Map.Entry<String, Object>> iterator = map.entrySet().iterator();
while (iterator.hasNext()) {
    Map.Entry<String, Object> next = iterator.next();
    System.out.println("key:" + next.getKey());
    System.out.println("value:" + next.getValue());
}
```



Map常用的实现类有`HashMap` 、`TreeMap` 两者差别不大，TreeMap 中的数据是有序的，遍历时数据是顺序遍历的



