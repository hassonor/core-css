## Flexbox

___

### What is Flexbox?

* A Set of CSS Properties
* Creating Flexible Layouts
* Distributing Extra Space
* Aligning Content

### The Flex Container

```css
.flex-container {
    display: inline-flex;
    border: solid 4px black;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo1.png)

### Flex Flow Direction

* By Default: Flex items flow left to right -> (This is the Main Axis)

```css
.flex-container {
    display: inline-flex;
    flex-direction: row-reverse;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo2.png)

```css
.flex-container {
    display: inline-flex;
    flex-direction: column;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo3.png)

```css
.flex-container {
    display: inline-flex;
    flex-direction: column-reverse;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo4.png)
