

- SwiftUI
- PickerStyle
-  segmented 

Type Property

# segmented

A picker style that presents the options in a segmented control.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
static var segmented: SegmentedPickerStyle { get }
```

Available when `Self` is `SegmentedPickerStyle`.

## Discussion

Use this style when there are two to five options. Consider using menu when there are more than five options.

For each option’s label, use sentence-style capitalization without ending punctuation, like a period or colon.

To apply this style to a picker, or to a view that contains pickers, use the pickerStyle(_:) modifier.

## See Also

### Getting built-in picker styles

static var automatic: DefaultPickerStyle

The default picker style, based on the picker’s context.

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

static var wheel: WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

