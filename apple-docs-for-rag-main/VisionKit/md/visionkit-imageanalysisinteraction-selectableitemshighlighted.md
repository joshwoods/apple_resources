

- VisionKit
- ImageAnalysisInteraction
-  selectableItemsHighlighted 

Instance Property

# selectableItemsHighlighted

A Boolean value that indicates whether the interaction highlights actionable text or data the analyzer detects in text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var selectableItemsHighlighted: Bool { get set }
```

## Discussion

The interaction object manages this property value for you. It sets this property to `false` if you set the analysis property or the activeInteractionTypes property to an empty set. Otherwise, it sets this property depending on whether a person toggles the Live Text button in the interface.

## See Also

### Querying the interface state

var liveTextButtonVisible: Bool

A Boolean value that indicates whether the Live Text button appears.

var isSupplementaryInterfaceHidden: Bool

A Boolean value that indicates whether the view hides supplementary interface objects.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

func hasSupplementaryInterface(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

