# SASS Mixin for Rounded Corners

```
@mixin rounded($radius:1em) {
-webkit-border-radius:$radius;
-moz-border-radius:$radius;
border-radius:$radius;
}

#somediv {
	background:$orange;
	padding:5px;
	@include rounded(1em);
}
```