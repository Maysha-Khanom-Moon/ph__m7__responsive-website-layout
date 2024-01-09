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
--> flex is uni-directional
--> flex used at parent element
- display: flex;

- #### justify-content
    - it works horizontally
    - flex-start(default), center, flex-end, space-between, space-around, space-evenly
- #### align-items
    - it works vertically
    - flex-start(default), flex-end, center

- #### flex-direction
    - row(default), column, column-reverse, row-reverse
    - for column: axes are interchanged their direction. anti-clockwise 90deg. so main axis is vertically and cross axis horizontally.

- #### flex-wrap
    - without wrap: element will shrinked. no scrollbar added
    - wrap: no shrinking. Go to the new line. For single element scrollbar added.
    - no-wrap, wrap, wrap-reverse

- display: flex; by default make the child element height according to large child height, if height is not declared

- #### gap
    - it just create gap between child following main axis. its not included to the parent's height

<br>


### extra
- if I put 'required" into the input element then browser auto-matically will notify the user to fill-up the input-bar before submit.
- to center a element: margin auto or position absolute or flexbox or grid
- if element width define by % then it never move by normal display: flex; justify-content.
    - solution: wrap whole element via a div and use flex at the parent element.
    - actually need space to move the element.
    - it also applicable for align-items.

<br>


## Grid layout
--> grid is bi-directional

- display: grid; it's not matter if i just use this line only

- #### grid-template-columns
    - : 200px 300px 400px; means 3 column will created. 1st column is 200px, 2nd is 300px and 3rd one is 400px. We can change the column number and column size
    - : repeat(3, 200px); means 3 column will created and every column is 200px
    - at the same time we can use both method.
    - : repeat(3, 5fr) 2fr 1fr; means total viewport will divided by (3*5+2+1=18) parts. Then each of 1st 3 column will be 5 parts, total 15 parts. Also 6th 4th column will be 2 parts and last 5th column will be 1 part. (fr: fraction)
    - : 200px auto 100px; means 1st column is 200px and last column is 100px. And 2nd column is the remaining part

- grid element distribution: left to right then go to the new line.

- #### grid-tamplate-rows
    - as it is like grid-tamplate-column

- #### justify-content
    - as it is like flexbox

- #### align-items
    - as it is like flexbox

