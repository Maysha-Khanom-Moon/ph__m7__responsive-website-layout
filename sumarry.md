# Responsive website layout
--> layout: which container will sit in which place on the website

## css unit
- px: absolute length. Although its not 100% fixed. It can be vary in difference device
- %: relative to the value of parent element
- em: relative to the font-size of the parent element
- rem: relative to font-size of the root element
    - in general 1 rem = 16px

- vh: viewport-height. equal to 1% of the height of the browser window size
- vw: viewport-width. equal to 1% of the width of the browser window size
- vmax: follow the maximum
- vmin: follow the minimum
    - if device width > height then vmax = vw, vmin = vh
    - if device height > width then vmax = vh, vmin = vw

#### absolute
- px, in, cm, mm, pt(points), pc(picas)

#### relative
- %, em, rem, ex, ch, vh, vw, vmax, vmin

<br>

## flexbox layout
--> flex used at parent element
- display: flex;

- #### justify-content
    - it works horizontally
    - flex-start(default), center, flex-end, space-between, space-around, space-evenly
- #### align-items
    - it works vertically
    - flex-start(default), flex-end, center
- #### flex-direction
    - flex is uni-directional
    - row(default), column, column-reverse, row-reverse
    - for column: axes are interchanged their direction. anti-clockwise 90deg. so main axis is vertically and cross axis horizontally.

- #### flex-wrap
    - without wrap: element will shrinked. no scrollbar added
    - wrap: no shrinking. Go to the new line. For single element scrollbar added.
    - no-wrap, wrap, wrap-reverse

- display: flex; by default make the child element height according to large child height, if height is not declared

- #### gap
    - it just create gap between child following main axis. its not included to the parent's height



### extra
- if I put 'required" into the input element then browser auto-matically will notify the user to fill-up the input-bar before submit.
- to center a element: margin auto or position absolute or flexbox or grid
- if element width define by % then it never move by normal display: flex; justify-content.
    