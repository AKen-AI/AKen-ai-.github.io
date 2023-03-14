# 线性查找-人类最直观的查找方式
线性查找应该是人类最容易思考的查找方式
举个例子，比如在你的班级里面一共有三十个人，已知他们来自祖国的大将南北，其中我们想找到一个来自新疆的人如何去找呢，我们最直观的想法就是进入教室，从第一排的座位开始，按照顺序一个一个的询问，只到我们找到来自新疆的同学

### Python实现

**使用Python内置方法**
```py{2}
all_student_location=["北京","上海","新疆","安徽","湖南"]
all_student_location.index("新疆") # Python内置方法
```

**传统算法逻辑实现**
```py{3}
def liner_search(li:list,v:int) -> int: 
    for i in range(len(li)+1):
        if li[i] == v:
            return i
    return None
```
