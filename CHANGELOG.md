# Change Log

## [1.7.0] - 2017-03-28
- Refactor sorting to fit Material Design spec. Allow to configure default sorting

## [1.6.0] - 2017-03-27
- Rewrite disabling row detail: use callback instead of data bindings

## [1.5.3] - 2017-03-22
- Fix wrong attribute on sort icon

## [1.5.2] - 2017-03-10
- Fix sort icon position when align-right is set to true, add TODO to refactor this

## [1.5.1] - 2017-03-06
- Fix case when splices are not propagated to data bindings

## [1.5.0] - 2017-03-01
- Expose headerHeight and rowMinHeight properties

## [1.4.5] - 2017-02-28
- Fix footer height and spinner positioning

## [1.4.4] - 2017-02-28
- Show spinner in footer when loading is set to true. Fixes #6
- Make disabled buttons lighter and allow to configure this

## [1.4.3] - 2017-02-27
- Handle case when there are no matching records after applying filter (#8)

## [1.4.2] - 2017-02-23
- Fix wrong CSS selector for left shadow

## [1.4.1] - 2017-02-22
- Expose hasPages property. Fix shadow position when table does not have pages

## [1.4.0] - 2017-02-21
- Implement pagination

## [1.3.4] - 2016-12-15
- Expose `initialCount` and `targetFramerate` properties of rows `dom-repeat` template

## [1.3.3] - 2016-12-05
- Add missing `polymer.html` import to hint Polymer.Templatizer behavior

## [1.3.2] - 2016-11-22
- Filtering items containing `null` or `undefined` values now work
- Empty (`""`) filters are now ignored when filtering items
- Filtering `false` values work now
- Add filtering tests

## [1.3.1] - 2016-11-15
- Call `notifyResize` after first rows render to fix appearance on Windows

## [1.3.0] - 2016-11-10
- Allow disabling details for particular rows via `detailDisabled` bound property

## [1.2.0] - 2016-11-07
- Make string sorting case-insensitive by default, add `sortCaseSensitive` option

## [1.1.4] - 2016-11-04
- Fix `_forwardParentPath`: propagate changes to all instances

## [1.1.3] - 2016-11-04
- Fix width calculating on resize / scroll events

## [1.1.2] - 2016-11-01
- Add missing `paper-ripple` dependency
- Add inline demo

## [1.1.1] - 2016-10-26
- Fix sort icon width by setting `flex-basis`

## [1.1.0] - 2016-10-24
- Rewrite sorting: sort on whole column header cell tap

## [1.0.2] - 2016-10-21
- Remove obsolete observer

## [1.0.1] - 2016-10-21
- Fix lint issues

## [1.0.0] - 2016-10-21
- Rewrite sorting: fix rendering issue, remove multi-column sorting

## [0.1.0] - 2016-10-12
- Initial release
