

- SwiftUI
- ControlGroupStyle
-  navigation 

Type Property

# navigation

The navigation control group style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var navigation: NavigationControlGroupStyle { get }
```

Available when `Self` is `NavigationControlGroupStyle`.

## Discussion

Use this style to group controls related to navigation, such as back/forward buttons or timeline navigation controls.

The navigation control group style can vary by platform. On iOS, it renders as individual borderless buttons, while on macOS, it displays as a separated momentary segmented control.

To apply this style to a control group or to a view that contains a control group, use the controlGroupStyle(_:) modifier.

## See Also

### Getting built-in control group styles

static var automatic: AutomaticControlGroupStyle

The default control group style.

static var compactMenu: CompactMenuControlGroupStyle

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

static var menu: MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

static var palette: PaletteControlGroupStyle

A control group style that presents its content as a palette.

