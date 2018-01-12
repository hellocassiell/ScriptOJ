### 转换驼峰命名
完成 toCamelCaseVar 函数，它可以接受一个字符串作为参数，可以把类似于 is_good 这样的变量名替换成 isGood。
```
const toCamelCaseVar = (variable) => /* TODO */
{
  return variable.replace(/_+[a-zA-Z]/g,(m, i) => {
  	if(i) return (m.match(/[a-zA-Z]/)[0].toUpperCase());
  	else return m;
  })
}
```