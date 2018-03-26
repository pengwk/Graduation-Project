# Matlab 技巧


## 动态绘制图形

#### 例子

```matlab
x=0;figure;plot(x,sin(x));hold on
for n=1:300
      x=n;
      plot(x,sin(x),'r.','MarkerSize',6);
      drawnow;
end
```

[来源:一个作图问题，如果做实时更新的plot？](http://www.ilovematlab.cn/thread-218787-1-1.html)

## 打印到控制台

#### disp

显示数组或文字内容。例子：

```matlab
name = 'Alice';   age = 12;
X = sprintf('%s will be %d this year.', name, age);
disp(X)

name = 'Alice';   age = 12;
X = fprintf('%s will be %d this year.\n', name, age);

X = '<a href = "http://www.mathworks.com">MathWorks Web Site</a>';
disp(X)
```

## 字符串处理


## 其他函数

- `print` 打印图像或者保存到文件
