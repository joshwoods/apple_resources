

- VisionKit
- ImageAnalysisInteraction
-  setSupplementaryInterfaceHidden(\_:animated:) 

Instance Method

# setSupplementaryInterfaceHidden(\_:animated:)

Hides or shows supplementary interface objects, such as the Live Action button and Quick Actions, depending on the item type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final func setSupplementaryInterfaceHidden(
    _ hidden: Bool,
    animated: Bool
)
```

## Parameters 

`hidden`  

`true` to hide the supplementary interface; otherwise, `false`.

`animated`  

`true` to animate the interface transition; otherwise, `false`.

## See Also

### Customizing the interface

var allowLongPressForDataDetectorsInTextMode: Bool

A Boolean value that indicates whether people can press and hold text to activate data detectors.

var supplementaryInterfaceContentInsets: UIEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: UIFont?

The font to use for the supplementary interface.

