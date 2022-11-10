# CSS - Responsive Grid + Spacing

An example of simple responsive grid in plain css.

## Elements

The grid system is based on 5 elements:

* [Containers](#containers)
* [Rows](#rows)
* [Columns](#columns)
* [Push columns](#push-columns)
* [Spacing](#spacing)

### Map of meaning

#### Sizes

* `xl` - this si an extra large (e**X**tra **L**arge) - **1200px**;
* `lg` - this si a large (**L**ar**G**e) - **992px**;
* `md` - this si a medium (**M**e**D**ium) - **768px**;
* `sm` - this si a small (**SM**all) - **576px**;

### Containers

There are 2 containers, but in general just 3 of them are used in the real world.

* `.container-full` - this container width is 100%;
* `.container` - this container width is 1200px (this width can be changed into grid.css file);

*The container will contain direct childs just rows not columns.*

### Rows

There is just one class with name row. 

* `.row` - this is the row inside the container or a col.

*The row class should be added as a child to the container or col. A container can have multiples rows.*

### Columns

The grid system is split into `12` columns. A row can have maximum of `12` columns.

The generic convention for columns class is:

`.col-{size}-{number}`
* `size` - it can be `xl`, `lg`, `md` or `sm`;
* `number` - it can be `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10`, `11` or `12`.

The `size` from columns will set the behaviour width of the responsive device.
The `number` from columns will set how many columns should be set for the specific width device. (12 column is the maximum used in the grid to form a row)

### Push columns

The push columns help to orgineze the columns if there is need of more space.

`.col-push-{size}-{number}`
* `size` - it can be `xl`, `lg`, `md` or `sm`;
* `number` - it can be `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10`, `11` or `12`.

The `size` from columns will set the behaviour width of the responsive device.
The `number` from columns will set how many columns should be set for the specific width device. (12 column is the maximum used in the grid to form a row)

Example:
`col-xl-6 col-push-xl-3` - this will create a col with 6 and it will push 3 column from left. So the col-xl-6 will be align in the center of the row.

### Spacing

The spacing are help classes and they can be used with col or into custom html tags.


`.{type}-{number}`

`.{type}-{axes}-{number}`

* `type` - it can be `m` from margin or `p` from padding;
* `axes` - it can be `t` from top, `r` from right, `b` from bottom, `l` from left, `x` for left and right, `y` for top and bottom. This use css box model axes. The axes are **optional**. If there is no axes in class name, the number will be applyed to all axes: top, right, bottom and left.
* `number` - the numbers are in px: `0`, `2`, `4`, `6`, `8`, `10`, `12`, `14`, `16`, `18`, `20`, `22`, `24`, `26`, `28`, `30`, `32`, `34`, `36`, `38` or `40`.

Example of margin:
* `m-t-10` - this will set a margin top of 10px;
* `m-r-10` - this will set a margin right of 10px;
* `m-b-10` - this will set a margin bottom of 10px;
* `m-l-10` - this will set a margin left of 10px;
* `m-x-10` - this will set a margin left and right of 10px;
* `m-y-10` - this will set a margin top and bottom of 10px;
* `m-10` - this will set a margin top, right, bottom and left of 10px;

Example of padding:
* `p-t-10` - this will set a padding top of 10px;
* `p-r-10` - this will set a padding right of 10px;
* `p-b-10` - this will set a padding bottom of 10px;
* `p-l-10` - this will set a padding left of 10px;
* `p-x-10` - this will set a padding left and right of 10px;
* `p-y-10` - this will set a padding top and bottom of 10px;
* `p-10` - this will set a padding top, right, bottom and left of 10px;


# License

[MIT](https://github.com/s3c4/angular-ts-math/blob/master/LICENSE) © [Andrei Secareanu](https://github.com/s3c4)

Made with :blue_heart: from London

