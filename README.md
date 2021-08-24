# Inputs

`data-icon` attribute is using [Material Icons](https://fonts.google.com/icons "Material icons reference")

## Text Input

- To disable input, simply add `disabled` to `<input>`
- `<label>` is optional
- Add `.rtlI` to `.tInput` when using **rtl** input

```html
<p class="tInput">
  <input type="text" id="ID" name="" placeholder="" />
  <label for="ID" data-icon="">The label</label>
</p>
```

JavaScript

```javascript
document.querySelectorAll(".tInput").forEach((tInput) => {
  new TInput(tInput);
});
```

## Checkbox / Radio

- To disable input, simply add `disabled` to `<input>`

Checkbox

```html
<div class="cInput">
  <input type="checkbox" name="" id="ID" />
  <label for="ID"><span class="label">The label</span></label>
</div>
```

JavaScript

```javascript
document.querySelectorAll(".cInput").forEach((cInput) => {
  new CInput(cInput);
});
```

Radio

```html
<div class="rInput">
  <input type="radio" id="ID" name="" />
  <label for="ID"><span class="label">The label</span></label>
</div>
```

JavaScript

```javascript
document.querySelectorAll(".rInput").forEach((rInput) => {
  new RInput(rInput);
});
```

## File Input

```html
<p class="fInput">
  <input id="ID" type="file" name="" multiple />
  <label for="ID" data-icon="">Choose File</label>
</p>
```

JavaScript

```javascript
document.querySelectorAll(".fInput").forEach((fInput) => {
  new FInput(fInput);
});
```
