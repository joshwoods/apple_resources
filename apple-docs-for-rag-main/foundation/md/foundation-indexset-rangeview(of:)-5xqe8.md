

- Foundation
- IndexSet
-  rangeView(of:) 

Instance Method

# rangeView(of:)

Returns a `Range`-based view of `self`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeView(of range: Range) -> IndexSet.RangeView
```

## Parameters 

`range`  

A subrange of `self` to view.

## See Also

### Getting a Range-Based View

var rangeView: IndexSet.RangeView

Returns a `Range`-based view of the entire contents of `self`.

struct RangeView

A view of the contents of an IndexSet, organized by range.

