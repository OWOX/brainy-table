[![Build Status](https://travis-ci.org/OWOX/brainy-table.svg?branch=master)](https://travis-ci.org/OWOX/brainy-table)
[![Bower version](https://badge.fury.io/bo/brainy-table.svg)](https://badge.fury.io/bo/brainy-table)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/OWOX/brainy-table)

_[Demo and API docs](https://owox.github.io/brainy-table/)_

# &lt;brainy-table&gt;

`brainy-table` is a Polymer 1.x data table element.

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="../iron-ajax/iron-ajax.html">
    <link rel="import" href="../iron-icon/iron-icon.html">
    <link rel="import" href="../iron-icons/iron-icons.html">
    <link rel="import" href="brainy-table.html">
    <div>
      <template is="dom-bind">
        <next-code-block></next-code-block>
      </template>
    </div>
  </template>
</custom-element-demo>
```
-->
```html
<iron-ajax auto url="demo/users.json" last-response="{{users}}"></iron-ajax>
<brainy-table items="[[users.data]]" page-size="5" details-enabled>
  <brainy-table-column name="First Name" filter-by="user.name.first" sort-by="user.name.first">
    <template>[[item.user.name.first]]</template>
  </brainy-table-column>
  <brainy-table-column name="Last Name" sort-by="user.name.last">
    <template>[[item.user.name.last]]</template>
  </brainy-table-column>
  <brainy-table-column name="Phone" sort-by="user.phone" align-right>
    <template>[[item.user.phone]]</template>
  </brainy-table-column>
  <brainy-table-column width="30px" align-right flex="0">
    <template>
      <template is="dom-if" if="[[!expanded]]">
        <iron-icon icon="icons:expand-more"></iron-icon>
      </template>
      <template is="dom-if" if="[[expanded]]">
        <iron-icon icon="icons:expand-less"></iron-icon>
      </template>
    </template>
  </brainy-table-column>
  <template is="row-detail">
    <div>[[item.user.location.street]], [[item.user.location.city]], [[item.user.location.state]]</div>
  </template>
  <div no-results>No records found</div>
</brainy-table>
```

Inspired by [iron-data-table](https://github.com/Saulis/iron-data-table).
Follows the guidelines of [Material Design](https://material.google.com/components/data-tables.html).

## Features
- Data filtering
- Data sorting
- Pagination
- Template support for each column
- Two-way binding support
- Custom styling support for templates
- Flex support for cells
- Native Shadow DOM support
- Column manipulation, resizing, hiding, reordering
- Custom header templates
- Row details
- Disabling row details depending on item subproperty value
- Horizontal scrolling shadows
- "Drag-and-drop" scroll

## Special use cases
- Limited amount of data (for infinite scrolling, consider using `iron-data-table` instead)
- Table shouldn't be explicitly sized (height depends on rows count)
- Rows can include dropdown menus etc (no `transform` is used, so table does not create `z-index` trap)
