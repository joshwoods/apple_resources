

- VisionKit
- ImageAnalysisOverlayView
-  isSupplementaryInterfaceHidden 

Instance Property

# isSupplementaryInterfaceHidden

A Boolean value that indicates whether the view hides supplementary interface objects.

macOS 13.0+

``` source
@MainActor
final var isSupplementaryInterfaceHidden: Bool { get set }
```

## Discussion

Supplementary interface objects include the Live Text button and the interface for Quick Actions, depending on the item type. Setting this property invokes the setSupplementaryInterfaceHidden(_:animated:) method, passing this property value and `true` for the animated parameter.

## See Also

### Querying the interface state

var liveTextButtonVisible: Bool

A Boolean value that indicates whether the Live Text button appears.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

func hasSupplementaryInterface(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

var selectableItemsHighlighted: Bool

A Boolean value that indicates whether the overlay view highlights actionable text or data that the analyzer detects in text.

