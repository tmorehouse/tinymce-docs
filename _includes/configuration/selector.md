## selector

This option allows you to specify a CSS selector for the areas that TinyMCE should make editable.

When using this option in TinyMCE's regular editing mode, the element will be replaced with an `iframe` that TinyMCE will perform all operations within.

**Types:**

* `String`: CSS selector matching the element(s) you want TinyMCE to be attached to

**Default Value:**

There is no default value for `selector` since it's a mandatory key. In order to instantiate TinyMCE you need to pass a valid CSS selector string that targets at least one `HTMLDomElement` in your page.

##### Example replace a `textarea` element with id `editable`

```js
tinymce.init({
  selector: 'textarea#editable'  // change this value according to your HTML
});
```

When using this option in TinyMCE's inline editing mode, the selector can be used on any block element and will edit the content in place instead of replacing the element with an `iframe`.

##### Example Inline editing mode on a `div` element with `id` `"editable"`

When using this option in TinyMCE's inline editing mode, the selector can be used on any block element and will edit the content in place instead of replacing the element with an `iframe`.

```js
tinymce.init({
  selector: 'div#editable',
  inline: true
});
```

For more information on the differences between regular and inline editing modes please see this page [here]({{ site.baseurl }}/get-started/use-tinymce-inline/).
