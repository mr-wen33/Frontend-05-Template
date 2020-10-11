学习笔记

1. break 跳出多层循环
```
outer:for (......) {
    for (......) {
        break outer;
    }
}
```