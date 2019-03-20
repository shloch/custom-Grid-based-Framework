# DESIGN YOUR OWN GRID-BASED FRAMEWORK

This project aims to create a replica of www.microverse.org  website.  
It is part of [Microverse](https://www.microverse.org/) curriculum.
## Contributors
  - Louis SHEY _https://github.com/shloch_
  - Fabien RAKOTOMAMPIANDRA _https://github.com/FabienNeibaf_

## USAGE
our CSS grid framework file is the file "tailor.scss"
It's a framework for building HTML building blocks and it revolves around the figure 12.
That means in a single row, you can build a maximum of 12-equallly-calculated, responsive columns. You could also build fewer blocks that have their widths summing up to the width of 12 blocks.

The basic formular for using the framework is demonstrated below

<div class="hbox">
    <div class="ds-4"></div>
    <div class="ds-4"></div>
    <div class="ds-4"><div>
</div>

The example above is an equal-sized 3-block horizontal grid. The class names of the children blocks should be of format "ds-X" (0 < X < 13), with the sum of different X not exceeding 12. All blocks should be wrapped in a parent block with a class of "hbox"

The framework has been built with media queries in mind for responsiveness with 4 breakpoints denoted with the following short caracters.

sm-X : small screens with width between 351px - 768px
md-X : medium screens with width between 768px - 992px
lg-X : large screens with width between 993px - 1250px
xl-X : extra large screens with minimum width of  1251px

X in these scenarios is also in the interval ==> (0 < X < 13)

The basic example above can be made responsive on medium and small screens as follows

<div class="hbox">
    <div class="ds-4 md-6 sm-12"></div>
    <div class="ds-4 md-6 sm-12"></div>
    <div class="ds-4 md-6 sm-12"><div>
</div>

Explanation : from above example, we have 3 equally split blocks placed horizontally to each other on a single row on normal(ds-X)  screens. 
- As we move to medium screens, like tablets (md-X), the block size moves to 6 (being half of 12, that makes 50%). Therefore, we shall have two blocks placed next to each other on row one and a third lonely block on row two occupying 50% of the row.
- As we move towards small screens (sm-X), we will have these 3 blocks, each on a separate row and each occupying fully the row width.


Additionally, you can also hide blocks you wish at particular breakpoints by using following self-explanatory classes.

sm-none : hide blocks at small screens with width between 351px - 768px
md-none : hide blocks at medium screens with width between 768px - 992px
lg-none : hide blocks at large screens with width between 993px - 1250px
xl-none : hide blocks at extra large screens with minimum width of  1251px

EXAMPLE :
<div class="hbox">
    <div class="ds-8 sm-12"></div>
    <div class="ds-4 sm-none"></div>
</div>

From exaple above, the second block is hidden (invisible) at small screens.





## Live demo
