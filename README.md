# tableFixedHeader
A simple JS method for creating a table with a fixed header that doesn't use floats or absolute positioning, or any special markup.
Start with a basic table structure, include thead element. Widths specified in the thead will be carried into the new "fixed" layout. The scrollbar width is taken into account if the table is larger than the specified height. (You must specify a table height in order to trigger scrolling and a fixed header.

Initialize:
tableFixedHeader(string table-elem, int height);
