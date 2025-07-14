

- VisionKit
- ImageAnalysisOverlayView
-  supplementaryInterfaceFont 

Instance Property

# supplementaryInterfaceFont

The font to use for the supplementary interface.

macOS 13.0+

``` source
@MainActor
final var supplementaryInterfaceFont: NSFont? { get set }
```

## Discussion

The interaction also uses the font weight for image symbols, but ignores the point size to keep button sizes consistent.

## See Also

### Customizing the interface

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Text button and the interface for Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: NSEdgeInsets

The distances the edges of content are inset from the supplementary interface.

struct MenuTag

Tags that enable your app to manage image-analysis context menu items.

