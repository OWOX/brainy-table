[![Build Status](https://travis-ci.org/web-padawan/brainy-table.svg?branch=master)](https://travis-ci.org/web-padawan/brainy-table)

# &lt;brainy-table&gt;

`brainy-table` is a Polymer 1.x data table element.

[Demo and API Docs](http://web-padawan.github.io/brainy-table/)

Inspired by [iron-data-table](https://github.com/Saulis/iron-data-table).
Follows the guidelines of [Material Design](https://material.google.com/components/data-tables.html).

## Features
- Data filtering
- Data sorting
- Multi-column sorting
- Template support for each column
- Two-way binding support
- Custom styling support for templates
- Flex support for cells
- Native Shadow DOM support
- Column manipulation, resizing, hiding, reordering
- Custom header templates
- Row details
- Horizontal scrolling shadows
- "Drag-and-drop" scroll

## Special use cases
- Limited amount of data (for infinite scrolling, consider using `iron-data-table` instead)
- Table shouldn't be explicitly sized (height depends on rows count)
- Rows can include dropdown menus etc (no `transform` is used, so table does not create `z-index` trap)
