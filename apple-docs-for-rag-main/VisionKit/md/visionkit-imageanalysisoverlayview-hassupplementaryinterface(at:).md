

- VisionKit
- ImageAnalysisOverlayView
-  hasSupplementaryInterface(at:) 

Instance Method

# hasSupplementaryInterface(at:)

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

macOS 13.0+

``` source
@MainActor
final func hasSupplementaryInterface(at point: CGPoint) -> Bool
```

## Parameters 

`point`  

A point in the image, in view coordinates.

## Return Value

`true` if supplementary interface objects exist at `point`; otherwise, `false`.

## Discussion

Supplementary interface objects include the Live Text button and Quick Actions, depending on the item type.

## See Also

### Querying the interface state

var liveTextButtonVisible: Bool

A Boolean value that indicates whether the Live Text button appears.

var isSupplementaryInterfaceHidden: Bool

A Boolean value that indicates whether the view hides supplementary interface objects.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

var selectableItemsHighlighted: Bool

A Boolean value that indicates whether the overlay view highlights actionable text or data that the analyzer detects in text.

