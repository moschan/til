# Adjacent selector

If you want to make separated manu of horizontal, you can use **Adjacent selector**.

### Example HTML


```html
<ul>
  <li>menu01</li>
  <li>menu02</li>
  <li>menu03</li>
  <li>menu04</li>
  <li>menu05</li>
</ul>
```

### Basic Example

```css
li {
  padding-left: .5em;
  display: inline-block;
  border-left: 2px solid #000;
}

li:first-child {
  border-left: none;
}
```


### Smart Example using Adjacent selector

```css
li {
  padding-left: .5em;
  display: inline-block;
}

li + li {
  border-left: 2px solid #000;
}
```

You can see example [here](http://codepen.io/moschan/pen/KVNRbR)
