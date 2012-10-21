# Simplr Gallery
An easy jQuery plugin to display a Flickr photoset as a gallery.

Simplr Gallery takes a Flickr photoset and makes a gallery to be displayed on any website.

## How Do I Use Simplr Gallery?
Include jQuery 1.7+ and jquery.simplrgallery.js in your layout.

```javascript
<script src="your/path/jquery.min.js" type="text/javascript"></script>
<script src="your/path/jquery.simplrgallery.js" type="text/javascript"></script>
```

Then open up the jquery.simplrgallery.js file and edit line 13 to match your Flickr API key.

```javascript
//***CHANGE THESE VALUES TO MATCH YOUR FLICKR CRITERIA***//
	var apiKey = 'YOUR_API_KEY';
//******************************************************//
```
Then in a javascript file call the simplrgallery function on the HTML element you wish to populate with the gallery, and pass it the photo set ID you want to display as well as any other option.

```javascript
<script type="text/javascript">
	$(document).ready(function(){
		$('#YOUR_ELEMENT').simplrgallery({photoSet:'PHOTO SET ID'});
	});
</script>
```

It is that easy!  When the page loads it will create a simple and basic gallery to display your Flickr photoset.

...But I don't like the way it looks.  That's ok because Simplr Gallery has options!

## The Options

Simplr Gallery has 5 options you can configure if you would like to customize it.

```javascript
<script type="text/javascript">
	$(document).ready(function(){
		$('#YOUR_ELEMENT').simplrgallery({
			photoSet:'PHOTO SET ID', //Just the photo set ID (Don't consider this an option, IT IS REQUIRED).
			thumbSelector:'ANYNAME', //This will add a custom ID that is specified to the thumbnail's parent element.
			photoSelector:'ANYNAME', //This will add a custom ID that is specified to the large single photo.
			photoSize:'medium', //Excepts one of three possible values 'small', 'medium', or 'large'.
			caption:true, //Excepts a boolen value (true or false).  Displays the image's title as the caption of the photo.
			externalCss:true //Excepts a boolen value (true or false).  Turns off built in styles so that an external style may be appiled.
		});
	});
</script>
```

## Changelog
+ `v 1.0` -Initial Release

## Credits
[Sean Gofus](http://www.seangofus.com) | @seangofus