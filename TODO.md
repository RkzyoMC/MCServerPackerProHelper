TODO List

## 1
> 只有在工作区，且执行初始化命令才启用
1.
- 读取 setting.yml 内 `work.suffixes` 键
```yaml
work:
  suffixes:
    - ".yml"
```
> 只有在指定的的文件后缀下运行

---

- 读取 registry.yml 内 `path` `expressions` 键
```yaml
paths:
  - "./default"
expressions:
  - "\\$\\(mcp\\.([^)]+)\\)"
```
> 只有在 `paths` 目录下的文件才扩展才工作

2. 屏蔽语法错误
如果语法错误划线部分满足`expressions`
屏蔽这个语法错误
