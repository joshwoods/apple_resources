

- UIKit
- UITitlebar
-  titleVisibility 

Instance Property

# titleVisibility

A value that indicates the visibility of the title.

Mac Catalyst 13.0+

``` source
@MainActor
var titleVisibility: UITitlebarTitleVisibility { get set }
```

## Mentioned in 

Removing the title bar in your Mac app built with Mac Catalyst

## Discussion

Setting the title visibility to UITitlebarTitleVisibility.hidden hides only the title displayed in the title bar, not the title bar itself. To remove the title bar from the window, set titleVisibility to UITitlebarTitleVisibility.hidden and toolbar to `nil`.

This property defaults to UITitlebarTitleVisibility.visible.

## See Also

### Configuring the title bar

var separatorStyle: UITitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

enum UITitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

enum UITitlebarTitleVisibility

States that determine visibility of the title in the title bar.

var representedURL: URL?

A URL of the file or resource represented in the window.

