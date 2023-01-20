# CSS Animations Transform

Transform targets the element's movement, size, rotate.

`transform` accept different values which includes `translate`, `scale`, `rotate` and few others.

### Translate

Moves the element from one place to another place. 

* `translate(x_axis, y_axis)` - moves the element in both left to right and top to bottom directions
* `translateX(x_axis)` - moves the element from left to right that is on x-axis
* `translateY(y_axis)` - moves the element from top to bottom that is on y-axis
* `NOTE:` all the positive `(+)` values indicates the forward direction and negative `(-)` values indicates backward direction. 

### Scale

Shrinks or expands the element.

* `scale(x_axis, y_axis)` - scaling for both the axis if the y-axis value is not provided, it consider x-axis value equal to y-axis
* `scaleX()` - scale in x-axis direction
* `scaleY()` - scale in y-axis direction
* `NOTE:` it accepts only numerical values as inputs and negative `(-)` value makes the element to get reverted in the respective axis.

### Rotate

Rotate the element. 

* `rotate()` - clockwise rotation in the z-axis. 
* `rotateX()` - clockwise rotation in the X axis, if the element is in the 2D plane it will shrink in the top and bottom axis.
* `rotateY()` - clockwise rotation in the Y axis, if the element is in the 2D plane it will shrink in the left and right axis.
* `rotateZ()` - clockwise rotation in the Z axis.
* `NOTE:` Negative `(-)` value rotate in opposite direction

We can have combination of all the three properties to an element.

```css
transform: rotateX(60deg) translateX(100px) scaleX(1.2);
```