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

时间复杂度：$\mathcal{O}(N l)$ 

<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ4MjgzNDYwLC0yMDg4NzQ2NjEyLC0yMD
g4NzQ2NjEyLC0xMjU4OTg1NjgsLTEwNzU0MDU2NTQsLTIwODg3
NDY2MTIsLTEzNzM4MDMzNzcsLTExMDc0NDA1NDhdfQ==
-->