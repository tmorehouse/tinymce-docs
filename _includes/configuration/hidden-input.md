## hidden_input

This option gives you the ability to disable the auto generation of hidden input fields for inline editing elements. By default all inline editors have a hidden input element in which content gets saved when an `editor.save()` or `tinymce.triggerSave()` is executed.

This can be disabled if you don't need these controls.

**Types:**

* `Boolean`: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

**Default Value:**

```js
true
````

**Possible Values:**

* `true`: enable the auto generation of hidden input fields for inline editing elements
* `false`: disable the auto generation of hidden input fields for inline editing elements

##### Example

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  inline: true,
  hidden_input: false
});
```
