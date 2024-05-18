# perosnal site
The way the math has been done to make the hexagon elements is to always split the viewport height in half first, each use that to compute some values like width factor, numberOfColumn values, which is used to create a grid cell, since we split the screen height in half so virtually there will always only be two rows for gridcells, gridcell is what houses hexagon elements within it.

so based on the number of columns the first row will have gridcells from 0 to numberofCOlumns-1, and second row will contain gridcells from numberOfColumns to numberOfColumns*2-1(because total number of grid cells that can be present in two rows will be 0 to 2*numberOfColumns, as each row gets numberOfColumns number of gridcell elements).

For any content one would want to put inside the hexagon, that content must be cut and sized as per the style mentioned in .sidebarelement, so that it fits and it is positioned at the centre of the hexagon.