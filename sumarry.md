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