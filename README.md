# BigFoot

一款高效脚本架构包，可用于油猴脚本等脚本的快捷开发。

## 快速上手

### 使用 ：
```
// ==UserScript==
// @name         BigFoot 
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       You
// @match        引入脚本包（脚本包地址）
// @icon         data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==
// @grant        none
// ==/UserScript==

(function() {
    'use strict';
	new Bigfoot({
		data: {
			text : "world"
		},
		async mounted() {
			this.consoleHello(this.text)
		},
		methods: {
			consoleHello(text){
				console.log("hello" + text)
			}
		}
	})
    // Your code here...
})();
```
## 说明

具体方法请查阅 
官方网站 http://bigfoot.renxingdao.work/
官方文档 https://www.kancloud.cn/shuaishuai_162/jb_tool/2680688



