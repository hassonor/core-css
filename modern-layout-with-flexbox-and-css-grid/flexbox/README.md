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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo1.png)
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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo2.png)
___

```css
.flex-container {
    display: inline-flex;
    flex-direction: column;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo3.png)
___

```css
.flex-container {
    display: inline-flex;
    flex-direction: column-reverse;
    border: solid 4px #000
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo4.png)
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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo5.png)
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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo6.png)
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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo6.png)
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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo7.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo8.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo9.png)

___

```css
.flex-container {
    display: flex;
    border: solid 4px #000;
    width: 55%;
    height: 30em;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo10.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo11.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_demo12.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo1.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo2.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo3.png)
![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo3_2.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo4.png)
![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo4_2.png)

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

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/display_order_demo5.png)
___

### Flexibility

___

#### Flex Grow Factor

Control how much a given item in a row or column will stretch relative to the other items <br>
within that row or column in order to fill up the positive free space. <br>
We can set the flex grow factor using `flex-grow` property.

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_grow_factor.png)

____
Without `flex-grow` property:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
}

.flex-item-01 {
    background-color: #A62E5C;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/without_flex_grow_property.png)
___
With `flex-grow` property:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    flex-grow: 1;
}

.flex-item-01 {
    background-color: #A62E5C;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/with_flex_grow_property.png)

___

One of the items to be larger than the others:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    flex-grow: 1;
}

.flex-item-01 {
    background-color: #A62E5C;
}

.flex-item-02 {
    background-color: #9BC850;
    flex-grow: 4;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/with_flex_grow_property_one_item_larger_than_others.png)

___

#### Flex Shrink Factor `flex-shrink`

This Property is the opposite of the `flex-grow` property.<br>
It controls how the space is distributed when there's not enough space for the items to fit.

Without `flex-shrink` property:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    with: 15em;
}

.flex-item-01 {
    background-color: #A62E5C;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_shrink_demo_1.png)

___

With `flex-shrink: 2` property on flex item 01:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    with: 15em;
}

.flex-item-01 {
    background-color: #A62E5C;
    flex-shrink: 2;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_shrink_demo_2.png)

___
With `flex-shrink: 0` property on flex item 01:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    with: 15em;
}

.flex-item-01 {
    background-color: #A62E5C;
    flex-shrink: 0;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_shrink_demo_3.png)

___

#### Initial Size (flex-basis)

___
Flex-basis sets the initial size of the items before the __extra__ space is _*distributed*_. <br>
It shares many similarities with the width property, and in fact even uses the exact same length values, <br>
meaning _*pixels*_, _*points*_, _*ems*_, _*rems*_ or _*percentages*_.
![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/initial_size.png)

___
Example without flex-basis:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
}

.flex-item-01 {
    background-color: #A62E5C;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/without_initial_size.png)

___

Example with `flex-basis: 10em` for flex-item-01:

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
}

.flex-item-01 {
    background-color: #A62E5C;
    flex-basis: 10em;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/with_flex_basis_demo_1.png)

__

Example with `flex-basis: 10em` for flex-item-01 and `flex-grow: 1` for flex-item.

```css
.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    flex-grow: 1;
}

.flex-item-01 {
    background-color: #A62E5C;
    flex-basis: 10em;
}

.flex-item-02 {
    background-color: #9BC850;
}

.flex-item-03 {
    background-color: #675BA7;
}

.flex-item-04 {
    background-color: #2A9FBC;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/with_flex_basis_demo_2.png)

__

Shorthand `flex: flex-grow flex-shrink flex-basis` <br> Example_1:

```css
.flex-container {
    display: flex;
    border: solid 4px #000;
    width: 50%;
}

.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    flex: 0 1 auto;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_shorthand_demo.png)

___

Shorthand `flex: flex-grow flex-shrink flex-basis` <br> Example_2:

```css
.flex-container {
    display: flex;
    border: solid 4px #000;
}

.flex-item {
    color: #fff;
    font-size: 1.2em;
    padding: 1em;
    text-align: center;
    flex: 0 0 auto;
}
```

![Twitter](https://github.com/hassonor/core-css/blob/master/screenshots/flex_shorthand_demo_2.png)

___