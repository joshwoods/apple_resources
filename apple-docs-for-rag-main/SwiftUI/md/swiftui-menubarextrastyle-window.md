

- SwiftUI
- MenuBarExtraStyle
-  window 

Type Property

# window

A menu bar extra style that renders its contents in a popover-like window.

macOS 13.0+

``` source
static var window: WindowMenuBarExtraStyle { get }
```

Available when `Self` is `WindowMenuBarExtraStyle`.

## Discussion

The styling and layout of controls is similar to that when contained in a normal window, compared to the menu-like layout that the menu style provides.

## See Also

### Getting menu bar extra styles

static var automatic: AutomaticMenuBarExtraStyle

The default menu bar extra style.

static var menu: PullDownMenuBarExtraStyle

A menu bar extra style that renders its contents as a menu that pulls down from the icon in the menu bar.

