# js-surprise

Some surprising functions for js

; 1
: 2
<details>
<summary>1. 日历</summary>
<pre>
创建过去七天的数组，如果将代码中的减号换成加号，你将得到未来7天的数组集合
[...Array(7).keys()].map(days => new Date(Date.now() - 86400000 * days));
</pre>
</code>
</details>

<details>
<summary>2. 生成随机ID</summary>
<pre>
// 生成长度为11的随机字母数字字符串
Math.random().toString(36).substring(2);
</pre>
</code>
</details>

<details>
<summary>3. 获取URL的查询参数</summary>
<pre>
// ?foo=bar&baz=bing => {foo: bar, baz: bing}
const q = {}
location.search.replace(/([^?&=]+)=([^&]+)/g, (_,k,v) => q[k] = v)
console.log(q)
</pre>
</code>
</details>