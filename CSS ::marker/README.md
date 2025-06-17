# problem with ::marker

The [`::marker`](https://developer.mozilla.org/en-US/docs/Web/CSS/::marker) is have the problems when using with class CSS selector.

```css
/* Working with global ::marker */
::marker {
  color: hsl(15, 53%, 34%);
}

/* Not working with class ::marker */
.others-best-food::marker {
  color: hsl(153, 53%, 34%);
}

```

The reason behind that is the `::marker` is always inside the `li` tag so the `.best-food::marker` will never reach.

The solution for that just using empty space selector

```css
.others-best-food ::marker {
  color: hsl(202, 53%, 34%);
}
```

or specific the marker inside the list

```css
.others-best-food li::marker {
  color: hsl(202, 53%, 34%);
}
```
