# jquery.links

Convert URL strings to HTML links quickly and easily.

## Usage

Simply select the element which contains the URL containing text and use the `.links()` method.

```html
<div class="message">Check out this wikipedia page! http://en.wikipedia.org/wiki/URL</div>
<script>
	$('div.message').links();
</script>
```

This will convert the contents of `div.message` to:

```html
Check out this wikipedia page! <a href="http://en.wikipedia.org/wiki/URL" target="_blank">http://en.wikipedia.org/wiki/URL</a>
```

If you want to specify a target other than `_blank`, you may specify it when running the `.links()` method:

```javascript
$('div.message').links({ target: 'other_target' });
```