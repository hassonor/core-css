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
___

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
___

```css
.flex-container {
    display: inline-flex;
    flex-direction: column;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo3.png)
___

```css
.flex-container {
    display: inline-flex;
    flex-direction: column-reverse;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo4.png)
___

### Flex Line Wrapping

```css
.flex-container {
    display: flex;
    flex-wrap: nowrap;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo5.png)
___

```css
.flex-container {
    display: flex;
    flex-wrap: wrap;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo6.png)
___

```css
.flex-container {
    display: flex;
    flex-wrap: wrap;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo6.png)
___

```css
.flex-container {
    display: flex;
    flex-wrap: wrap-reverse;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo7.png)

___

```css
.flex-container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo8.png)

___

```css
.flex-container {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column-reverse;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo9.png)

___

```css
.flex-container {
    display: flex;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo10.png)

___

```css
.flex-container {
    display: flex;
    flex-flow: column wrap;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo11.png)

___

```css
.flex-container {
    display: flex;
    flex-flow: row-reverse wrap-reverse;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/flex_demo12.png)

___