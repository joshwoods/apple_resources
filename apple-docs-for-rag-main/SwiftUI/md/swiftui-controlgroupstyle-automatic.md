

- SwiftUI
- ControlGroupStyle
-  automatic 

Type Property

# automatic

The default control group style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var automatic: AutomaticControlGroupStyle { get }
```

Available when `Self` is `AutomaticControlGroupStyle`.

## Discussion

The default control group style can vary by platform. By default, both platforms use a momentary segmented control style that’s appropriate for the environment in which it is rendered.

You can override a control group’s style. To apply the default style to a control group or to a view that contains a control group, use the controlGroupStyle(_:) modifier.

## See Also

### Getting built-in control group styles

static var compactMenu: CompactMenuControlGroupStyle

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

static var menu: MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

static var navigation: NavigationControlGroupStyle

The navigation control group style.

static var palette: PaletteControlGroupStyle

A control group style that presents its content as a palette.

