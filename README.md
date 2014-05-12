magic
=====

CSS3 Animations with special effects. Now on beta, more effects coming soon. Many thanks to [daneden](http://daneden.me/animate/) for inspiration!
My next step is to minifing the code.
Take a look at the demo [NEW DEMO PAGE](http://minimamente.com/example/magic_animations/)

##Installation


Include magic.css

Example:
```html
<link rel="stylesheet" href="dist/magic.min.css">
```

##Usage

This is a sample code on hover with jQuery, first you include the class "magictime" and after your desired animation.
```js
$('.yourdiv').hover(function () {
  $(this).addClass('magictime puffIn');
});
```

If you want to load the animation after certain time, you can use this example:
```js
//set timer to 5 seconds, after that, load the magic animation
setTimeout(function(){
  	$('.yourdiv').addClass('magictime puffIn');
}, 5000);
```

If you want to load the animation after certain time but with infinite loop, you can use this example:
```js
//set timer to 3 seconds, after that, load the magic animation and repeat forever
setInterval(function(){
	$('.yourdiv').toggleClass('magictime puffIn');
}, 3000 );
```

You can change the time of the animation by set the class "magictime" for example:
```css
.magictime {
-webkit-animation-duration: 3s;
animation-duration: 3s;
}
```

Default CSS timing is:
```css
.magictime {
-webkit-animation-duration: 1s;
animation-duration: 1s;
}
```
