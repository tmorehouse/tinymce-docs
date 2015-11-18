## toolbar

This option allows you to define toolbars and specify the buttons and the order that they will appear in the editor. Many [plugins]({{ site.baseurl }}/plugins/) will make available new buttons that can be added to the toolbar.

**Types:**

* `String`: A space separated list of toolbar controls. To create groups within this list, please add `|` pipe characters between the groups of controls that you would like to create.
* `Boolean`: To disable the toolbar, the toolbar option should be provided a boolean value of `false`.
* `Array`: To specify multiple toolbars, the toolbar option should be provided with an array of space separated strings, see `String` above.

**Default Value:**

```js
'insertfile undo redo | styleselect | bold italic | alignleft aligncenter alignright alignjustify | bullist numlist outdent indent | link image'
```

##### Example grouped toolbar

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  toolbar: 'undo redo | styleselect | bold italic | link image'
});
```

##### Disabling the toolbar Example

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
    toolbar: false
});
```

##### Example using multiple toolbars

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  toolbar: [
    'undo redo | styleselect | bold italic | link image',
    'alignleft aligncenter alignright'
  ]
});
```

Alternatively, you may specify multiple toolbars through the use of the [toolbar(n)](#toolbarn) option.
