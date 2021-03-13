```python
# 列表
# 创建列表
a = ["hello","world","every"]
# 访问列表
print(a[0])
print(a[1])
print(a[2])
# 列表遍历
for i in a:
    print(i)
# 列表加法
b = [4,5,6]
c = a + b#[1,2,3,4,5,6] 列表的加法也表示的是拼接
# 列表乘法
print(a * 2)
# 在列表中添加元素 在列表末尾添加:append("要添加的元素") 在指定的位置插入insert(索引值,"要添加的元素")
a.append("lalal")
a.insert(0,"lalal")
# 在列表中删除元素 删除指定位置的元素pop(位置)，删除指定的元素remove(指定元素)
a.pop(0)
a.remove("lalal")
# 求列表的长度len(列表名)
print(len(a))
# 判断数据在不在列表中，会输出 True False
print(1 in a)
# 列表切片的结果一定是列表，不能和字符串比较大小
print(a[:1])
print(a[0])
# 最大值，最小值max(列表名) min(列表名)
print(max(a))
print(min(a))
# 列表改变排序 a.sort()从小到大 a.reverse()列表翻转 a.sort(reverse = True)从大到小 ，三个操作都是改变的原先列表的顺序，没有生成新的列表
m = sorted(a)#生成新的列表，而且是从小到大排序好的列表
# # 把字符串转化成列表 list(字符串)
c = list("hello")
print(c)







```
