

- UIKit
- UIFocusItemContainer
-  focusItems(in:) 

Instance Method

# focusItems(in:)

Retrieves all of the focus items within this container that intersect with the provided rectangle.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
func focusItems(in rect: CGRect) -> [any UIFocusItem]
```

**Required**

## Parameters 

`rect`  

The rectangle used to look for focus items that intersect the rectangle expressed in the container’s coordinate space.

## Return Value

An array of focus items that intersect the provided rectangle. The focus items are expressed in the container’s coordinate space.

## Discussion

The found focus items should report their frames in the coordinateSpace.

## See Also

### Retrieving focus items

var coordinateSpace: any UICoordinateSpace

The coordinate space of the focus items contained in the focus item container.

**Required**

