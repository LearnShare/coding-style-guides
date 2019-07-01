# EditorConfig

<https://editorconfig.org/>

## 语法

.editorconfig

```ini
# 注释语法

# 最高优先级
root = true

# 应用到所有文件
[*]
end_of_line = lf

# 应用到 .js 文件
[*.js]
charset = utf-8

# 应用到指定类型的文件
[*.{html,css}]

# 应用到指定目录
[lib/**.js]

# 应用到指定文件
[{app.js,config.json}]
```

## 匹配规则

| 语法 | 匹配规则 |
|---|---|
| `*` | 匹配任何字符串，除了 `/` |
| `**` | 匹配任何字符串 |
| `?` | 匹配任何字符 |
| `[name]` | 匹配 'name' 中的任何字符 |
| `[!name]` | 匹配不在 'name' 中的任何字符 |
| `{s1,s2,s3}` | 匹配列表中的任意字符串（以逗号分隔） |
| `{num1..num2}` | 匹配位于 'num1' 至 'num2' 之间的任意整数 |

## 规则

### indent_style

缩进风格

+ tab
+ space

### indent_size

缩进数量

+ 正整数
+ tab 使用 tab_width

### tab_width

tab 宽度

+ 正整数

### end_of_line

行尾序列

+ lf
+ crlf
+ cr

### charset

字符集

+ latin1
+ utf-8
+ utf-16be
+ utf-16le
+ utf-8-bom

### trim_trailing_whitespace

清除末尾空白符

+ true 开启
+ false 关闭

### insert_final_newline

末尾插入空行

+ true 开启
+ false 关闭

### max_line_length

每行最大字符数

+ 正整数
+ off 关闭

## 模板

```ini
root = true

[*.{ts,js,html,css,scss,less}]
charset = utf-8
indent_style = space
indent_size = 2
tab_width = 2
end_of_line = lf
trim_trailing_whitespace = true
insert_final_newline = true
max_line_length = 80
```
