CSS GRID

Vocabulary

Functions
repeat()
minmax()

Display
grid ~ generates a block-level grid
inline ~ grid - generates an inline-level grid

grid-template-columns: px | fr | % | auto  (width)
grid-template-rows: px | fr | % | auto  (height)
grid-template-area



Set Up

.container {
  display: grid | inline-grid;
  grid-template-columns: 100px auto 100px | 1fr auto 1fr | repeat(3, 1fr | 
    repeat( 3, minmax( 100px, 1fr)) (width)
  grid-template-rows: 50px 500px |  (height)
  grid-gap: 3px
}

Responsive

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-template-rows: 100px 200px
  height: 100%;
}




Explicit ~ rows/cols that have been defined
Implicit ~ rows/cols that have not been defined, or rows/cols that will be added at a future time

Justify items ~ Justifies the individual grid areas horizontally, because it works on the inline or row axis. Justify items will go in the grid container/wrapper.
Justify self ~ Justifies the itmes inside of the grid containers horizontally. Used with grid items.
values: auto | normal | start | end | center | stretch | baseline | first baseline | last baseline

Align items ~ Aligns the individual grid areas vertically, because it works on the block or column axis. Align items will go in the grid container/wrapper.
Align self ~ Aligns the items inside of a grid area. Used with grid items. 
values: auto | normal | start | end | center | stretch | baseline | first baseline | last baseline

  *justify and align self are applied to areas e.g. header, footer, etc.
  *justify and align items are applied to body elements e.g. containers
  *adjusting these items effect their child elements as well.

Flex vs Grid
*you can display:flex to create and position navbar elements by using nth-child(). See Scrimba tutorial "Grid vs Flex"
