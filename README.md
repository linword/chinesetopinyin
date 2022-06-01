# chinesetopinyin
中文转拼音，顾名思义，就是将中文词语或者句子转化为英文，不支持多音字。

# | 用法

### 1.如果在node环境下使用：

```powershell
node pytranslate.js
```

​		<font color='red'>js代码中还包含nodejs的语法，用于windows自动复制转化后的结果，如果不需要，比如在html中引用该js，请在代码中注释自动复制的代码。如果需要其他系统自动复制的功能，代码中注释的语句中有包括说明。</font>

### 2.在html里引用：

```javascript
/**
 * pinyin.getCamelChars(str, boolean)转拼音首字母
 * @param  {String}   str      要转拼音的字符串
 * @param  {Boolean}  boolean  true为大写，false为小写
 */
/**
 * pinyin.getFullChars(str, boolean, type)转拼音全拼
 * @param  {String}   str      要转拼音的字字符串
 * @param  {Boolean}  boolean  true为拼音首字母大写，false为拼音首字母小写
 * @param  {String}   type     type为"space"时，拼音以空格分隔
 */

//转拼音首字母大写
pinyin.getCamelChars("测试", true); //CS
//转拼音首字母小写
pinyin.getCamelChars("测试", false); //cs
//转拼音全拼且首字母大写，且不会以空格分隔
pinyin.getFullChars("测试", true); //CeShi
//转拼音全拼且全是小写，且不会以空格分隔
pinyin.getFullChars("测试", false); //ceshi
//转拼音全拼且首字母大写，且以空格分隔
pinyin.getFullChars("测试", true, "space"); //Ce Shi
//转拼音全拼且全是小写，且以空格分隔
pinyin.getFullChars("测试", false, "space"); //ce shi
```

如果需要实现其他需求，请自行更改，欢迎交流！

代码demo链接地址：[中文转拼音 (linmew.xyz)](https://linmew.xyz/tools/chinesetpy/)

代码有些是根据网上来进行改写的，如果有问题，请发邮件至[linmew@vip.qq.com](mailto:linmew@vip.qq.com)，收到邮件后会联系处理。

