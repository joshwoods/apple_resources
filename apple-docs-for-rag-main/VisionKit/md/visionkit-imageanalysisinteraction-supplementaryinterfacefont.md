

- VisionKit
- ImageAnalysisInteraction
-  supplementaryInterfaceFont 

Instance Property

# supplementaryInterfaceFont

The font to use for the supplementary interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var supplementaryInterfaceFont: UIFont? { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

The interaction also uses the font weight for image symbols, but ignores the point size to keep button sizes consistent.

## See Also

### Customizing the interface

var allowLongPressForDataDetectorsInTextMode: Bool

A Boolean value that indicates whether people can press and hold text to activate data detectors.

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Action button and Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: UIEdgeInsets

The distances the edges of content are inset from the supplementary interface.

