# common-regex
常用正则表达式

### IP
```
((?:(?:25[0-5]|2[0-4]\d|[01]?\d?\d)\.){3}(?:25[0-5]|2[0-4]\d|[01]?\d?\d))
```

### 域名
`https://www.qq.com`  
```
^((http:\/\/)|(https:\/\/))?([a-zA-Z0-9]([a-zA-Z0-9\-]{0,61}[a-zA-Z0-9])?\.)+[a-zA-Z]{2,6}(\/)
```

### QQ
```
[1-9]([0-9]{5,11})
```

### 国内固话号码
`XXX-XXXXXXX` `XXXX-XXXXXXXX` 固定电话
```
(\(\d{3,4}\)|\d{3,4}-|\s)?\d{8}
```

### 手机号码
13513213258
```
^1(3|4|5|6|7|8|9)\d{9}$
```

### username
字母开头，允许5-16字节，允许字母数字下划线
```
^[a-zA-Z][a-zA-Z0-9_]{4,15}$
```

### email
只允许英文字母、数字、下划线、英文句号、以及中划线组成
```
^[a-zA-Z0-9_-]+@[a-zA-Z0-9_-]+(\.[a-zA-Z0-9_-]+)+$
```

### 汉字
```
^[\u4e00-\u9fa5]{0,}$
```

### 英文和数字
```
^[A-Za-z0-9]+$
```

### 禁止输入含有%&',;=?$"等字符
```
[^%&',;=?$\x22]+
```

## 参考
- [cdoco/common-regex](https://github.com/cdoco/common-regex)  
- [fighting41love/funNLP](https://github.com/fighting41love/funNLP)  
- [VincentSit/ChinaMobilePhoneNumberRegex](https://github.com/VincentSit/ChinaMobilePhoneNumberRegex) - 一组匹配中国大陆手机号码的正则表达式
