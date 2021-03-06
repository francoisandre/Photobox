Photobox v2.0.7
===============

Welcome to Photobox, a lightweigth image displaying jQuery module.
[Demo](http://codepen.io/GKlein/full/QEGXpz/)

----------


Documentation
----------------------

Using Photobox is really **easy**!

1 - Install with Bower:
```
bower install photobox-js
```

2 - Add these lines at the right place in your document:

- In the header:
```html
<link rel="stylesheet" href="bower_components/photobox-js/dist/css/photobox.min.css">
```

- In the body:
```html
<img src="path/to/your/image" rel="photobox" title="anything you want">
```
and/or
```html
<a href="path/to/your/image" rel="photobox" title="anything you want">
```

> You can create albums by adding *data-pb-album* attribute to the element (data-pb-album="myAlbum")

- At the end of the body:
```html
<script src="bower_components/jquery/dist/jquery.min.js"></script>
<script src="bower_components/photobox-js/dist/js/photobox.min.js">

/* Initialize Photobox */
<script>
	Photobox.init();
</script>
```

Add the attribute data-pb-album="Your album name" to group images.

You can pass options like this:
```html
<script>
	Photobox.init({
		opacity: "0.8",
		duration: "500"
	});
</script>
```

| Option       | Type | Default | Description                |
|--------------|------|---------|----------------------------|
| *duration* | millisecond | 500 | Opening animation duration |
| *opacity* | float | 0.7 | Opacity of the background (Between 0 and 1) |
| *player* | boolean | false | Activate the player |
| *interval* | millisecond | 500 | Duration between frames (For player) |
| *wrapAround* | boolean | false | After the last image of an album you will go back to the first image |

> **Tip:** Don't forget to import jQuery **before** Photobox.

