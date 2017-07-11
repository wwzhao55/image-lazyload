# image-lazyload
实现图片懒加载，优化性能
</br>
懒加载的主要目的是作为服务器前端的优化，减少请求数或延迟请求数

</br>
Web 图片的懒加载就是通过读取img元素，然后获得img元素的data-src（也可以约定为其他属性名）属性的值，并赋予img的src，从而实现动态加载图片的机制。

这里需要注意的是： img在初始化的时候不要设置src属性，因为即使设置 src=’’ 浏览器也会尝试加载图片。
</br>

  	页可见区域宽： document.body.clientWidth;
	</br>
	网页可见区域高： document.body.clientHeight;
	</br>
	网页可见区域宽： document.body.offsetWidth (包括边线的宽);
	</br>
	网页可见区域高： document.body.offsetHeight (包括边线的宽);
	</br>
	网页正文全文宽： document.body.scrollWidth;
	</br>
	网页正文全文高： document.body.scrollHeight;
	</br>
	网页被卷去的高： document.body.scrollTop;
	</br>
	网页被卷去的左： document.body.scrollLeft;
	</br>
	网页正文部分上： window.screenTop;
	</br>
	网页正文部分左： window.screenLeft;
	</br>
	屏幕分辨率的高： window.screen.height;
	</br>
	屏幕分辨率的宽： window.screen.width;
	</br>
	屏幕可用工作区高度： window.screen.availHeight;
	</br>
