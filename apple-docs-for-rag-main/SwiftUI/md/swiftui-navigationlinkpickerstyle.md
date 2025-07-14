

- SwiftUI
-  NavigationLinkPickerStyle 

Structure

# NavigationLinkPickerStyle

A picker style represented by a navigation link that presents the options by pushing a List-style picker view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct NavigationLinkPickerStyle
```

## Overview

In navigation stacks, prefer the default menu style. Consider the navigation link style when you have a large number of options or your design is better expressed by pushing onto a stack.

You can also use navigationLink to construct this style.

## Topics

### Creating the picker style

init()

Creates a navigation link picker style.

## Relationships

### Conforms To

- PickerStyle

## See Also

### Supporting types

struct DefaultPickerStyle

The default picker style, based on the picker’s context.

struct InlinePickerStyle

A `PickerStyle` where each option is displayed inline with other views in the current container.

struct MenuPickerStyle

A picker style that presents the options as a menu when the user presses a button, or as a submenu when nested within a larger menu.

struct PalettePickerStyle

A picker style that presents the options as a row of compact elements.

struct RadioGroupPickerStyle

A picker style that presents the options as a group of radio buttons.

struct SegmentedPickerStyle

A picker style that presents the options in a segmented control.

struct WheelPickerStyle

A picker style that presents the options in a scrollable wheel that shows the selected option and a few neighboring options.

