

- VisionKit
- ImageAnalysisInteraction
-  liveTextButtonVisible 

Instance Property

# liveTextButtonVisible

A Boolean value that indicates whether the Live Text button appears.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var liveTextButtonVisible: Bool { get }
```

## Discussion

When a person taps the Live Text button, it highlights recognized items in the image.

## See Also

### Querying the interface state

var isSupplementaryInterfaceHidden: Bool

A Boolean value that indicates whether the view hides supplementary interface objects.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

func hasSupplementaryInterface(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

var selectableItemsHighlighted: Bool

A Boolean value that indicates whether the interaction highlights actionable text or data the analyzer detects in text.

