

- Shared With You
- SWAttributionView
-  supplementalMenu 

Instance Property

# supplementalMenu

A supplemental menu to augment the attribution view’s existing menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var supplementalMenu: UIMenu? { get set }
```

**macOS**

``` source
@MainActor
var supplementalMenu: NSMenuItem? { get set }
```

## Discussion

Use `supplementalMenu` when there are additional actions a user can take on content represented by this view’s SWHighlight. A `nil` value informs the system to not add a supplemental menu.

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

var preferredMaxLayoutWidth: CGFloat

A width the system uses to constrain the view contents.

