

- VisionKit
- ImageAnalysisOverlayView
-  setSupplementaryInterfaceHidden(\_:animated:) 

Instance Method

# setSupplementaryInterfaceHidden(\_:animated:)

Hides or shows supplementary interface objects, such as the Live Text button and the interface for Quick Actions, depending on the item type.

macOS 13.0+

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

var supplementaryInterfaceContentInsets: NSEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: NSFont?

The font to use for the supplementary interface.

struct MenuTag

Tags that enable your app to manage image-analysis context menu items.

