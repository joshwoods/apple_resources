

- Shared With You
- SWAttributionView
-  highlightMenu 

Instance Property

# highlightMenu

A menu with a list of system actions specific to this hightlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var highlightMenu: UIMenu { get }
```

**macOS**

``` source
@MainActor
var highlightMenu: NSMenu { get }
```

## Discussion

Use this menu to augment an existing menu that the system attaches to the content represented by this SWAttributionView. This menu allows the user to reply to or hide the highlight. Your app needs to add this `hightlightMenu` inline with, and at the end of, the menu elements it augments.

## See Also

### Customizing highlights

var backgroundStyle: SWAttributionView.BackgroundStyle

The background style of the child view that contains names and avatars.

var displayContext: SWAttributionView.DisplayContext

The context for the content the system displays with this view.

var highlight: SWHighlight?

The highlight you use to display this attribution.

var horizontalAlignment: SWAttributionView.HorizontalAlignment

The horizontal alignment of the view.

var menuTitleForHideAction: String?

A localized string the system uses as a custom title for the hide menu item.

var preferredMaxLayoutWidth: CGFloat

A width the system uses to constrain the view contents.

var supplementalMenu: UIMenu?

A supplemental menu to augment the attribution view’s existing menu.

