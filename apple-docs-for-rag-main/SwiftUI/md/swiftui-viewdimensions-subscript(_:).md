

- SwiftUI
- ViewDimensions
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Gets the value of the given horizontal guide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
subscript(guide: HorizontalAlignment) -> CGFloat { get }
```

Show all declarations

## Overview

Find the offset of a particular guide in the corresponding view by using that guide as an index to read from the context:

```
.alignmentGuide(.leading) { context in
    context[.leading] - 10
}
```

For information about using subscripts in Swift to access member elements of a collection, list, or, sequence, see Subscripts in *The Swift Programming Language*.

## See Also

### Accessing guide values

subscript(explicit:)

Gets the explicit value of the given horizontal alignment guide.

