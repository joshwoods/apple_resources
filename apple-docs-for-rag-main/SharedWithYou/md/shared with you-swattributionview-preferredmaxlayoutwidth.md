

- Shared With You
- SWAttributionView
-  preferredMaxLayoutWidth 

Instance Property

# preferredMaxLayoutWidth

A width the system uses to constrain the view contents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var preferredMaxLayoutWidth: CGFloat { get set }
```

## Discussion

When embedding this view in a SwiftUI UIViewRepresentable or NSViewRepresentable view, the system constrains its contents to the `preferredMaxLayoutWidth` width.

If you’re not using SwiftUI this property shouldn’t be necessary, as SWAttributionView otherwise derives the maximum width from the frame or constraints you set.

## See Also

### Customizing highlights

var backgroundStyle: SWAttributionView.BackgroundStyle

The background style of the child view that contains names and avatars.

var displayContext: SWAttributionView.DisplayContext

The context for the content the system displays with this view.

var highlight: SWHighlight?

The highlight you use to display this attribution.

var highlightMenu: UIMenu

A menu with a list of system actions specific to this hightlight.

var horizontalAlignment: SWAttributionView.HorizontalAlignment

The horizontal alignment of the view.

var menuTitleForHideAction: String?

A localized string the system uses as a custom title for the hide menu item.

var supplementalMenu: UIMenu?

A supplemental menu to augment the attribution view’s existing menu.

