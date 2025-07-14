

- SwiftUI
- ControlGroupStyle
-  compactMenu 

Type Property

# compactMenu

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var compactMenu: CompactMenuControlGroupStyle { get }
```

Available when `Self` is `CompactMenuControlGroupStyle`.

## Discussion

To apply this style to a control group, or to a view that contains control groups, use the controlGroupStyle(_:) modifier.

## See Also

### Getting built-in control group styles

static var automatic: AutomaticControlGroupStyle

The default control group style.

static var menu: MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

static var navigation: NavigationControlGroupStyle

The navigation control group style.

static var palette: PaletteControlGroupStyle

A control group style that presents its content as a palette.

