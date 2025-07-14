

- Foundation
- IndexSet
-  rangeView 

Instance Property

# rangeView

Returns a `Range`-based view of the entire contents of `self`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rangeView: IndexSet.RangeView { get }
```

## See Also

### Getting a Range-Based View

func rangeView(of: Range&lt;IndexSet.Element>) -> IndexSet.RangeView

Returns a `Range`-based view of `self`.

struct RangeView

A view of the contents of an IndexSet, organized by range.

