官网 ： https://huangjunneng.github.io/



gitbook build


规范一级目录
mkdir src release test doc example
src —— 源码
release —— 发布结果
test —— 单元测试用例
doc —— 文档
example —— 示例

# 写文档
* 安装gitbook，然后创建SUMMARY.md文档目录
```js
npm i gitbook-cli -g
```
执行生成文档目录：
gitbook init
将md文档转换成html文档
gitbook build

启动本地服务预览上
gitbook serve
