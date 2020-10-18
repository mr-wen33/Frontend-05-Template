学习笔记

广度优先搜索使用队列完成，代码模式为
```
function bfs() {
    let que = [];
    while (que.length) {
        // 取出队头
        const father = que.shift();
        // 对队头的节点进行访问
        // ...
        // 然后将字节点放入队列，等待下一次循环访问
        que.push(father.children);
    }
}
```