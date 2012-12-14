jquery async upload plugin
easy to use

    // 上传方法
	$.upload({
			// 上传地址
			url: '/admin/upload', 
			// 文件域名字
			fileName: 'filedata', 
			// 其他表单数据
			params: {name: 'pxblog'},
			// 上传完成后, 返回json, text
			dataType: 'json',
			// 上传之前回调,return true表示可继续上传
			onSend: function() {
					return true;
			},
			// 上传之后回调
			onComplate: function(data) {
					alert(data);
			}
	});