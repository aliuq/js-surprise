# js-surprise

Some surprising functions for js

<details>
<summary>日历</summary>
// 创建过去七天的数组，如果将代码中的减号换成加号，你将得到未来7天的数组集合<br />
<code>
[...Array(7).keys()].map(days => new Date(Date.now() - 86400000 * days));
</code>
</details>
