### 1.
> `.`匹配除换行符以外的任意字符 </br>
`\w` 匹配字母或数字</br>
`\s` 匹配任意的空白符</br>
`\d` 匹配数字</br>
`\b` 匹配单词的开始或结束</br>
`^` 匹配字符串的开始</br>
<code>$</code> 匹配字符串的结束</br>

***
### 2.
>如果你想查找特殊代码本身的话，比如你查找.,或者*,就出现了问题：你没法指定它们，因为它们会被解释成其它的意思。
这时你就必须使用\来取消这些字符的特殊意义。因此，你应该使用`\.`和`\*`。当然，要查找\本身，你也得用`\\.`

***
### 3.
>`*`重复零次或更多次</br>
`+`重复一次或更多次</br>
`?`重复零次或一次</br>
`{n}`重复n次</br>
`{n,}`重复n次或更多次</br>
`{n,m}`重复n到m次</br>

***
### 4.
>`\W`匹配任意不是字母和数字的字符</br>
`\S`匹配任意不是空白符的字符</br>
`\D`匹配任意非数字的字符</br>
`\B`匹配不是单词开头或结束的位置</br>
`[^x]`匹配除了`x`以外的任意字符</br>
`[^aeiou]`匹配除了`aeiou`这几个字母以外的任意字符

***
### 5.
>`(exp)`匹配exp,并捕获文本到自动命名的组里</br>
`(?<name>exp)` 匹配exp,并捕获文本到名称为name的组里</br>
`(?:exp)` 匹配exp,不捕获匹配的文本</br>
**位置指定**</br>
`(?=exp)` 匹配exp前面的位置</br>
`(?<=exp)` 匹配exp后面的位置</br>
`(?!exp)` 匹配后面跟的不是exp的位置</br>
`(?<!exp)` 匹配前面不是exp的位置</br>
**注释**</br>
`(?#comment)` 这种类型的组不对正则表达式的处理产生任何影响，只是为了提供让人阅读注释

****
### 6.
>`*?`重复任意次，但尽可能少重复</br>
`+?` 重复1次或更多次，但尽可能少重复</br>
`??` 重复0次或1次，但尽可能少重复</br>
`{n,m}?` 重复n到m次，但尽可能少重复</br>
`{n,}?` 重复n次以上，但尽可能少重复</br>

转载自[https://blog.csdn.net/hz_lizx/article/details/55211104](https://blog.csdn.net/hz_lizx/article/details/55211104)
