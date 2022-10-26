# Css

**Content**
- [set up a dynamic grid based on flex](#issue-1)

<a name="issue-1"></a>
## set up a dynamic grid based on flex

```css
.container {
  border: 1px solid;
  display: inline-flex;
  flex-wrap: wrap; /* enable the wrap */
  margin:5px;
  vertical-align: top;
  width: 150px;
  height: 150px;
}

.container > * {
  flex-basis: 50%; /* width = 50% */
  flex-grow: 1; /* grow if alone in the last row */
  border: 1px solid red;
  box-sizing: border-box;
}
```

```html
<div class="container">
  <div></div>
</div>
<div class="container">
  <div></div>
  <div></div>
</div>
<div class="container">
  <div></div>
  <div></div>
  <div></div>
</div>
<div class="container">
  <div></div>
  <div></div>
  <div></div>
  <div></div>
</div>
```
