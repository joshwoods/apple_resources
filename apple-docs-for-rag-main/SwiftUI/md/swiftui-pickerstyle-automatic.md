

- SwiftUI
- PickerStyle
-  automatic 

Type Property

# automatic

The default picker style, based on the picker’s context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var automatic: DefaultPickerStyle { get }
```

Available when `Self` is `DefaultPickerStyle`.

## Discussion

How a picker using the default picker style appears largely depends on the platform and the view type in which it appears. For example, in a standard view, the default picker styles by platform are:

- On iOS and watchOS the default is a wheel.

- On macOS, the default is a pop-up button.

- On tvOS, the default is a segmented control.

The default picker style may also take into account other factors — like whether the picker appears in a container view — when setting the appearance of a picker.

You can override a picker’s style. To apply the default style to a picker, or to a view that contains pickers, use the pickerStyle(_:) modifier.

## See Also

### Getting built-in picker styles

static var inline: InlinePickerStyle

A `PickerStyle` where each option is displayed inline with other views in the current container.

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

