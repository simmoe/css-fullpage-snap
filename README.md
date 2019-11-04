# css-fullpage-snap

"CSS Scroll Snap is a module of CSS that introduces scroll snap positions, which enforce the scroll positions that a scroll container’s scrollport may end at after a scrolling operation has completed."
**MDN**

In human words, scroll snapping let's you control how your page scrolls between different sections. The basic concpt is simple: you give a scroll container (ie the body element) 

```css
body {
  scroll-snap-type: x mandatory;
  scroll-snap-type: y mandatory;
}
```
..where x and y represents the scroll direction. Then you give some elements on your page a scroll snap property:
```html
section{
  scroll-snap-align: center;
}
```

And you´re good to go. If needed you can add enforcement to the scroll stops:
```html
section{
  scroll-snap-align: center;
  scroll-snap-stop: always;
}
```
The last is not supported by all browsers, but it should.
