> Collection 是最基本的集合接口，一个Collection代表一组Object，即Collection的元素，java不提供直接继承自Collection的类，只提供继承于的子接口（如List和Set）。
>
> Collection 接口存储一组不唯一，无序的对象

Collection中提供的接口：

| 接口                                     | 描述                                         |
| ---------------------------------------- | -------------------------------------------- |
| size(): int                              | 返回集合的大小                               |
| contain(Object): boolean                 | 判断集合是否包含对象                         |
| containsAll(Collection<?>): boolean      | 集合中包含目标集合的所有元素                 |
| iterator(): Iterator<E>                  | 返回集合中元素的迭代器，不保证返回元素的顺序 |
| toArray(): Object[]                      | 集合转变为数组                               |
| toArray(T[]): T[]                        | 集合转变为对应类型的数组                     |
| add(E): boolean                          | 往集合中添加一个元素                         |
| addAll(Collection<? extends E>): boolean | 将指定集合的所有元素添加到此集合中           |
| remove(Object): boolean                  | 从集合中移除一个元素                         |
| removeAll(Collection<?>): boolean        | 移除集合中的所有也包含在指定集合中的元素     |
| removeIf(Predicate<? super E>): boolean  | 移除集合中所有符合要求的元素（1.8）          |
| retainAll(Collection<?>): boolean        | 从集合中移除所有不包含在指定集合中的元素     |
| clear(): void                            | 清除集合                                     |
| stream(): Stream                         | 返回此集合的处理流（1.8）                    |

