# CSS Animations Transition

Transition will transits the element from one state to another state. 

We can use below properties to achieve transition.

`transition` - shorthand to write below four properties into single line

1. `transition-duration`
    * set the duration for how many seconds or milliseconds a transition effect completes
    * accepts only integer values

2. `transition-property`
    * set name of the CSS property to apply transition
    * accepts all the name of CSS properties.

3. `transition-timing-function`
    * set the speed curve of transition effect 
    * accepts the values which includes
        * `linear` - same speed of transition from start to end
        * `ease` - slow start, then fast, then end slowly
        * `ease-in` - slow start, then fast
        * `ease-out` - fast start, then slow end
        * `ease-in-out` - slow start and end
4. `transition-delay`
    * set the delay of the transition
    * accepts only integer values 

We can achieve transition like below example. 

```css
.circle {
    transition-duration: 3s;
    transition-property: background, transform, box-shadow;
    transition-timing-function: ease-in;
    transition-delay: 1s;
}
```

`NOTE:` we can combine both `transition` and `transform`.

We can write the `transition` shorthand for the above example. 

```css
transition: background 1s 1s linear, transform 1s 1s ease-in, box-shadow 1s 1s ease-out;
```
* the pattern of shorthand is `transition: [transition-property] [transition-duration] [transition-delay] [transition-timing-function]`