# js-surprise

Some surprising functions for js

[^_^ //]: # (1 日历)
<details>
<summary>1. 日历</summary>
<pre>
创建过去七天的数组，如果将代码中的减号换成加号，你将得到未来7天的数组集合
[...Array(7).keys()].map(days => new Date(Date.now() - 86400000 * days));
</pre>
</code>
</details>

[^_^ //]: # (2 生成随机ID)
<details>
<summary>2. 生成随机ID</summary>
<pre>
// 生成长度为11的随机字母数字字符串
Math.random().toString(36).substring(2);
</pre>
</code>
</details>

[^_^ //]: # (3 获取URL的查询参数)
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

[^_^ //]: # (4 本地时间)
<details>
<summary>4. 本地时间</summary>
<pre>
new Date().toLocaleString()
</pre>
</code>
</details>

[^_^ //]: # (5 数组混淆)
<details>
<summary>5. 数组混淆</summary>
<pre>
const fn = arr => arr.slice().sort(() => Math.random() - 0.5)
console.log(fn([1,2,3,4,5]))
</pre>
</code>
</details>

[^_^ //]: # (6 生成随机十六进制代码,生成随机颜色)
<details>
<summary>6. 生成随机十六进制代码,生成随机颜色</summary>
<pre>
// 生成随机十六进制代码 如：'#c618b2'
'#' + Math.floor(Math.random() * 0xffffff).toString(16).padEnd(6, '0');
</pre>
</code>
</details>

[^_^ //]: # (7 数组去重)
<details>
<summary>7. 数组去重</summary>
<pre>[...new Set(arr)]</pre>
</code>
</details>

[^_^ //]: # (8 创建特定大小的数组)
<details>
<summary>8. 数组创建特定大小的数组去重</summary>
<pre>[...Array(3).keys()]</pre>
</code>
</details>

[^_^ //]: # (9 返回一个键盘)
<details>
<summary>9. 返回一个键盘</summary>
<pre>
(_=>[..."`1234567890-=~~QWERTYUIOP[]\\~ASDFGHJKL;'~~ZXCVBNM,./~"].map(x=>(o+=`/${b='_'.repeat(w=x&lt;y?2:' 667699'[x=["BS","TAB","CAPS","ENTER"][p++]||'SHIFT',p])}\\|`,m+=y+(x+'    ').slice(0,w)+y+y,n+=y+b+y+y,l+=' __'+b)[73]&&(k.push(l,m,n,o),l='',m=n=o=y),m=n=o=y='|',p=l=k=[])&&k.join`
`)()
</pre>
</code>
</details>