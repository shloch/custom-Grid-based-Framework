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



## Live demo
