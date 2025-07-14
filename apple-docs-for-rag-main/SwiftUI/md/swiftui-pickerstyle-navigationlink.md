

- SwiftUI
- PickerStyle
-  navigationLink 

Type Property

# navigationLink

A picker style represented by a navigation link that presents the options by pushing a List-style picker view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var navigationLink: NavigationLinkPickerStyle { get }
```

Available when `Self` is `NavigationLinkPickerStyle`.

## Discussion

In navigation stacks, prefer the default menu style. Consider the navigation link style when you have a large number of options or your design is better expressed by pushing onto a stack.

To apply this style to a picker, or to a view that contains pickers, use the pickerStyle(_:) modifier.

## See Also

### Getting built-in picker styles

static var automatic: DefaultPickerStyle

The default picker style, based on the picker’s context.

static var inline: InlinePickerStyle

A `PickerStyle` where each option is displayed inline with other views in the current container.

static var menu: MenuPickerStyle

A picker style that presents the options as a menu when the user presses a button, or as a submenu when nested within a larger menu.

static var palette: PalettePickerStyle

A picker style that presents the options as a row of compact elements.

static var radioGroup: RadioGroupPickerStyle

A picker style that presents the options as a group of radio buttons.

static var segmented: SegmentedPickerStyle

A picker style that presents the options in a segmented control.

static var wheel: WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

