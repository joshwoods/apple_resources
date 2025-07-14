

- VisionKit
- ImageAnalysisInteraction
-  isSupplementaryInterfaceHidden 

Instance Property

# isSupplementaryInterfaceHidden

A Boolean value that indicates whether the view hides supplementary interface objects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var isSupplementaryInterfaceHidden: Bool { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

Supplementary interface objects include the Live Text button and Quick Actions, depending on the item type. Setting this property invokes the setSupplementaryInterfaceHidden(_:animated:) method, passing this property value and `true` for the `animated` parameter.

## See Also

### Querying the interface state

var liveTextButtonVisible: Bool

A Boolean value that indicates whether the Live Text button appears.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

func hasSupplementaryInterface(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

var selectableItemsHighlighted: Bool

A Boolean value that indicates whether the interaction highlights actionable text or data the analyzer detects in text.

