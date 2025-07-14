

- VisionKit
- ImageAnalysisInteraction
-  allowLongPressForDataDetectorsInTextMode 

Instance Property

# allowLongPressForDataDetectorsInTextMode

A Boolean value that indicates whether people can press and hold text to activate data detectors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var allowLongPressForDataDetectorsInTextMode: Bool { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

If you set this property to `true` when the interaction type is just text, people can press and hold data in text, even when data detectors aren’t active. Otherwise, people can perform only text actions, such as copy and translate. The default value for this property is `true`.

## See Also

### Customizing the interface

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Action button and Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: UIEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: UIFont?

The font to use for the supplementary interface.

