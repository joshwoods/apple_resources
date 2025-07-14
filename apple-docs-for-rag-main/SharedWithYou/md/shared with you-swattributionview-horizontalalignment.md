

- Shared With You
- SWAttributionView
-  horizontalAlignment 

Instance Property

# horizontalAlignment

The horizontal alignment of the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var horizontalAlignment: SWAttributionView.HorizontalAlignment { get set }
```

## Discussion

This `horizontalAlignment` specifies the horizontal anchor for the view’s contents. This value only has an effect when the width of the contents are less than the available width. You should specify a value, in case the internal default ever changes.

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

var menuTitleForHideAction: String?

A localized string the system uses as a custom title for the hide menu item.

var preferredMaxLayoutWidth: CGFloat

A width the system uses to constrain the view contents.

var supplementalMenu: UIMenu?

A supplemental menu to augment the attribution view’s existing menu.

