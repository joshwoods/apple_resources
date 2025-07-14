

- UIKit
- UIFocusItemContainer
-  coordinateSpace 

Instance Property

# coordinateSpace

The coordinate space of the focus items contained in the focus item container.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
var coordinateSpace: any UICoordinateSpace { get }
```

**Required**

## Discussion

The focus items returned by focusItems(in:) should report their frames in this coordinate space.

## See Also

### Retrieving focus items

func focusItems(in: CGRect) -> [any UIFocusItem]

Retrieves all of the focus items within this container that intersect with the provided rectangle.

**Required**

