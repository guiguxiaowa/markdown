```cpp
bool is_prime(int n) {
    if (n == 1) {
        return false; // 不是质数
    }
    for (int i = 2; i * i <= n; i++) {
        if (n % i == 0) {
            return false; // 不是质数
        }
    }
    return true; // 是质数
}
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc3Mjc0NTMwNSwtMjA4ODc0NjYxMiwtMj
A4ODc0NjYxMiwtMTI1ODk4NTY4LC0xMDc1NDA1NjU0LC0yMDg4
NzQ2NjEyLC0xMzczODAzMzc3LC0xMTA3NDQwNTQ4XX0=
-->