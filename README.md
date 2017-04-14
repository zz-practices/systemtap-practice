# systemtap-practice
systemtap practice

## 安装
* CentOS
  ```
  curl https://raw.githubusercontent.com/WALL-E/static/master/setup/redhat/install_systemtap|bash
  ```

## 测试
```
# 测试stap
stap -V

# 测试kernel-debuginfo
stap -L 'kernel.function("printk")'

# 测试glibc-debuginfo
stap -L 'process("/lib64/libc.so.6").function("malloc")'
```
