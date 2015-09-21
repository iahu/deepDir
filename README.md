#deepDir - node module

深度遍历文件夹。可按文件类型过滤文件。


##安装

npm install deep-dir

##用法

```javascript
argvs.forEach(function(path){
	deepDir(path, {
		filters: {
			'.css' : cssFilter,
			'.js': jsFilter,
			'.html': htmlFilter
		},
		depth: depth // depth int型 遍历深度,0表示不限制深度
	});
});

function cssFiler(path) {
	console.log(path);
}
```