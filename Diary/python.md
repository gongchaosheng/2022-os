# 切片的参数列表
`s[start: end :step]`
+ 不省略参数的条件下，切片先考虑start到end的顺序，这个顺序如果是从左到右，step就必须为正，否则是空集,也就是step的方向要和从start到end的顺序相同  
```
s = '123abcdef'
b = s[0:5:-1]
print(b)
```
结果为空
```
b = s[0:5:1]
print(b)
```
结果为`123ab`
+ 切片若省略了参数。start和end都没有默认参数，只取决于step的方向  
```
b = s[0::1]
print(b)
```
省略了end，不用管end了，step是正数所以向右切片，结果为'123abcdef'
b = s[0::-1]
print(b)
#省略了end，不用管end了，step是负数所以向坐切片，结果为'1'






