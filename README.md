# move-cmp

## Project setup
```
pnpm install
```

### Compiles and hot-reloads for development
```
pnpm run serve
```

### Compiles and minifies for production
```
pnpm run build
```

### 文件结构

```
主包
    组件
        CMPA
        CMPB
    页面
        index，引用：CMPA

分包
    组件
        CMPC
    页面
        pageA，引用：CMPB、CMPC、CMPD
            组件
                CMPD
        pageB，引用：CMPB、CMPC
```

预期：

- CMPA：只有主包引用，不移动
- CMPB：被子包引用，移动到pageA、pageB中
- CMPC：被子包引用，引动到paeA、pageB中
- CMPD：被相应子包引用，不移动