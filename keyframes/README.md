# CSS Animations Keyframes

Keyframes are used to define the animations to the elements.

Steps to achieve keyframes animation.

1. Define the animation rule using `@keyframes`.
    * `@keyframes` - used to define a rule which consists of `from` and `to` blocks
    * `from` - used to define the starting properties inside the `@keyframes` animation block
    * `to` - used to define the ending properties inside the `@keyframes` animation block
    * We can also use `0%` instead of `from` and `100%` instead of `to`.

    ```css
    @keyframes drive {
        from {
            transform: translateX(0px);
        }
        to {
            transform: translateX(1365px);
        }
    }
    ```

2. Use the defined animation using `animation` property to a particular element. 
    * `animation` - used to write shorthand for below properties 
    * `animation-name` - accepts the name of `@keyframes` rule 
    * `animation-duration` - used to define the animation time 
    * `animation-iteration-count` - used to define the count of animation loop
    * `animation-direction`
        * used to define the direction of animation
        * accepts below values
            * `normal` - moves in forward direction
            * `reverse` - moves in backward direction
            * `alternate` - moves in forward and backward direction
    * `animation-timing-function`
        * used to define the speed of start and end positions
        * accepts below values
            * `linear` - same speed of transition from start to end
            * `ease` - slow start, then fast, then end slowly
            * `ease-in` - slow start, then fast
            * `ease-out` - fast start, then slow end
            * `ease-in-out` - slow start and end
    * `animation-delay` - used to define animation delay time

    ```css
    .bike {
        animation-name: drive;
        animation-duration: 5s;
        animation-iteration-count: infinite;
        animation-direction: reverse;
        animation-delay: 2s;
    }
    ```

`animation` shorthand
```css
animation: drive 2s linear infinite alternate;
```
* `NOTE:` we can assign more than one `@keyframes` rules to the `animation` property with the help of comma `(,)` separated values. 