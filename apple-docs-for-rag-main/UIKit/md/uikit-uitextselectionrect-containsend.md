

- UIKit
- UITextSelectionRect
-  containsEnd 

Instance Property

# containsEnd

A Boolean value that indicates whether the rectangle contains the end of the selection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var containsEnd: Bool { get }
```

## Discussion

The value of this property is used to determine the placement of the selection handles in bidirectional text. It provides a clue to the system about whether the end of the selection is in the specified rectangle.

## See Also

### Determining the Selection Status

var containsStart: Bool

A Boolean value that indicates whether the rectangle contains the start of the selection.

