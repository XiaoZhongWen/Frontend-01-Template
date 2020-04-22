### Number 直接量

```javascript
/^(\.\d+|(0|[1-9]\d*)\.?\d*)([eE][+-]?\d+)?$|^0[b|B][01]+$|^0[o|O][0-7]+$|^0[x|X][0-9a-fA-F]+$/
```

### UTF-8 Encoding 的函数

```javascript
function UTF8Encoding(str) {
  return str
    .split('')
    .map((s) => `\\u${s.charCodeAt().toString(16)}`)
    .join('')
}
```

### 字符串直接量

```javascript
/^u([0-9a-fA-F]{4}|\{(10|0?[0-9a-fA-F])[0-9a-fA-F]{0,4}\})$|^x[0-9a-fA-F]{2}$|^0(?!=\d)$|^[^\n\r\u2028\u2029\dxu]$/u
```

