

- SwiftUI
- PickerStyle
-  inline 

Type Property

# inline

A `PickerStyle` where each option is displayed inline with other views in the current container.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var inline: InlinePickerStyle { get }
```

Available when `Self` is `InlinePickerStyle`.

## See Also

### Getting built-in picker styles

static var automatic: DefaultPickerStyle

The default picker style, based on the picker’s context.

static var menu: MenuPickerStyle

A picker style that presents the options as a menu when the user presses a button, or as a submenu when nested within a larger menu.

static var navigationLink: NavigationLinkPickerStyle

A picker style represented by a navigation link that presents the options by pushing a List-style picker view.

static var palette: PalettePickerStyle

A picker style that presents the options as a row of compact elements.

static var radioGroup: RadioGroupPickerStyle

A picker style that presents the options as a group of radio buttons.

static var segmented: SegmentedPickerStyle

A picker style that presents the options in a segmented control.

static var wheel: WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

