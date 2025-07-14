

- SwiftUI
-  PickerStyle 

Protocol

# PickerStyle

A type that specifies the appearance and interaction of all pickers within a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol PickerStyle
```

## Topics

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

static var segmented: SegmentedPickerStyle

A picker style that presents the options in a segmented control.

static var wheel: WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

### Supporting types

struct DefaultPickerStyle

The default picker style, based on the picker’s context.

struct InlinePickerStyle

A `PickerStyle` where each option is displayed inline with other views in the current container.

struct MenuPickerStyle

A picker style that presents the options as a menu when the user presses a button, or as a submenu when nested within a larger menu.

struct NavigationLinkPickerStyle

A picker style represented by a navigation link that presents the options by pushing a List-style picker view.

struct PalettePickerStyle

A picker style that presents the options as a row of compact elements.

struct RadioGroupPickerStyle

A picker style that presents the options as a group of radio buttons.

struct SegmentedPickerStyle

A picker style that presents the options in a segmented control.

struct WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

### Deprecated styles

struct PopUpButtonPickerStyle

A picker style that presents the options as a menu when the user presses a button.

Deprecated

## Relationships

### Conforming Types

- DefaultPickerStyle
- InlinePickerStyle
- MenuPickerStyle
- NavigationLinkPickerStyle
- PalettePickerStyle
- PopUpButtonPickerStyle
- RadioGroupPickerStyle
- SegmentedPickerStyle
- WheelPickerStyle

## See Also

### Styling pickers

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

protocol DatePickerStyle

A type that specifies the appearance and interaction of all date pickers within a view hierarchy.

