## 筛法判定质数
```cpp
for (int i = 2; i <= n; i++) {
    is_prime[i] = true;
}
for (int i = 2; i * i <= n; i++) {
    if (is_prime[i]) {
        for (int j = i * i; j <= n; j +=i) {
             is_prime[j] = false;
        }
    }
}
```

时间复杂度：$\mathcal{O}(N \log \log N)$ 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI3NDI4NDQzNCwtMjA4ODc0NjYxMiwtMj
A4ODc0NjYxMiwtMTI1ODk4NTY4LC0xMDc1NDA1NjU0LC0yMDg4
NzQ2NjEyLC0xMzczODAzMzc3LC0xMTA3NDQwNTQ4XX0=
-->