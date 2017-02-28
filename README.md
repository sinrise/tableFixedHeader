# tableFixedHeader
A simple JS method for creating a table with a fixed header that doesn't use floats or absolute positioning, or any special markup.
Start with a basic table structure, including a thead element. Widths specified in the thead will be carried into the new "fixed" layout. The scrollbar width is taken into account if the table is larger than the specified height.

* Initialize:
  * $(string element).tableFixedHeader(int height, bool showFooter);

* Height:
  * optional
  * default: 300px
  * Height of table (body table must have a hiehgt in order to trigger scrolling. If the sum of the height of all the rows is smaller than the specified height, scrolling will not be triggered.

* ShowFooter:
  * optional
  * default: false
  * Displays a duplicate of the header at the bottom of the table, for tables so tall that you scroll past the header on the page. This is an edge case, as the whole point of having a fixed header is solve scrolling issues. However, there may be a case when you want a limits height table AND want it to scroll with a fixed header.
