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

### Display Order

* __For Visual Purposes Only__
* __Not For Logical Reordering__

___

### Example:

__Source Order__

```html

<div class="flex-container">
    <div class="flex-item">
        1
    </div>
    <div class="flex-item">
        2
    </div>
    <div class="flex-item">
        3
    </div>
</div>
```

![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo1.png)

___

```css
.flex-item-01 {
    background-color: #686868;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
    order: 0;
}

.flex-item-05 {
    background-color: #F15B2A;
}

.flex-item-06 {
    background-color: #9BC850;
}

.flex-item-07 {
    background-color: #BC2525;
}

.flex-item-08 {
    background-color: #dc3c3c;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo2.png)

___

```css
.flex-item-01 {
    background-color: #686868;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
    order: 1;
}

.flex-item-05 {
    background-color: #F15B2A;
}

.flex-item-06 {
    background-color: #9BC850;
}

.flex-item-07 {
    background-color: #BC2525;
}

.flex-item-08 {
    background-color: #dc3c3c;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo3.png)
![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo3_2.png)

___

```css
.flex-item-01 {
    background-color: #686868;
}

.flex-item-02 {
    background-color: #9BC850;
    order: 1;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
    order: 1;
}

.flex-item-05 {
    background-color: #F15B2A;
}

.flex-item-06 {
    background-color: #9BC850;
}

.flex-item-07 {
    background-color: #BC2525;
}

.flex-item-08 {
    background-color: #dc3c3c;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo4.png)
![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo4_2.png)

___

```css
.flex-item-01 {
    background-color: #686868;
}

.flex-item-02 {
    background-color: #9BC850;
    order: -1;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
    order: 1;
}

.flex-item-05 {
    background-color: #F15B2A;
}

.flex-item-06 {
    background-color: #9BC850;
}

.flex-item-07 {
    background-color: #BC2525;
}

.flex-item-08 {
    background-color: #dc3c3c;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/display_order_demo5.png)
___