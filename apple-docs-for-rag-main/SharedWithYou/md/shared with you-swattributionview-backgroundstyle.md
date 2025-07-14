

- Shared With You
- SWAttributionView
-  backgroundStyle 

Instance Property

# backgroundStyle

The background style of the child view that contains names and avatars.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var backgroundStyle: SWAttributionView.BackgroundStyle { get set }
```

## Discussion

If you don’t specify a background style, the system chooses one automatically. In general, SWAttributionView.BackgroundStyle.color looks best on monochrome backgrounds, while SWAttributionView.BackgroundStyle.material looks better on colored backgrounds.

## See Also

### Customizing highlights

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

var preferredMaxLayoutWidth: CGFloat

A width the system uses to constrain the view contents.

var supplementalMenu: UIMenu?

A supplemental menu to augment the attribution view’s existing menu.

