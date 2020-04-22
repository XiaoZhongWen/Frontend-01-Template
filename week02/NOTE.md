# 每周总结可以写在这里

1. Atom

   - Grammar

     - WhiteSpace(尽量不使用除空格

       ```
       <SP>
       ```

       以外的空白符 TIPS: 多种换行符的出现其实是因为老式打字机的问题 )

       - `: \t`
       - `: \v`
       - `: \f`
       - `: \s`
       - `：NO-BREAK SPACE`
       - `：ZERO WIDTH NO-BREAK SPACE`
       - ``

     - LineTerminator

       - `: \n`
       - `: \r`
       - ``
       - ``

     - Comment

       - `// comment 单行注释`
       - `/* comment */ 多行注释`

     - Token

       - IdentifierName
         - Keywords (关键字)
         - Identifier (标识符)
         - Future reserved Keywords: enum(枚举类型)
       - Punctuator
       - Template
       - Literal

   - Runtime

     - Types
       - Symbol 通常用来实现一些私有变量或唯一值
       - Number
         - 浮点数精度比较: Math.abs(0.1 + 0.2 - 0.3) < Number.EPSILON (这个式子有bug 1.1+1.3-2.4无法正确判断)
       - String
         - Code Point: U+0000 ~ U+10FFFF， 最好使用 U+0000 ~ U+FFFF范围内字符
       - Boolean
       - Undifined 在一些低版本浏览器undefined的值可以被重写
       - Null 这里有个历史遗留问题是typeof null 返回object的原因是因为js采用了低位存储 以000开头的变量会被typeof认为是object 而null表示都是0 所以会错误的被识别为object
       - BigInt 数字以n结尾 可以表示超出安全范围的数字(暂未进入标准)
     - Execution Context(执行上下文)

2. Expression

   - Atom
   - Operator
   - Punctuator

3. Statement

   - Expression
   - Keyword
   - Punctuator

4. Structure

   - Function
   - Class
   - Process
   - Namespace

5. Program/Module

   - Program
   - Module
   - Package
   - Library