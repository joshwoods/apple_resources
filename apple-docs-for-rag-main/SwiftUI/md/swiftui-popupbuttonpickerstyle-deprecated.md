

- SwiftUI
-  PopUpButtonPickerStyle Deprecated

Structure

# PopUpButtonPickerStyle

A picker style that presents the options as a menu when the user presses a button.

macOS 10.15–15.4Deprecated

``` source
struct PopUpButtonPickerStyle
```

Deprecated

Use MenuPickerStyle instead.

## Overview

Use this style when there are more than five options. Consider using RadioGroupPickerStyle when there are fewer than five options.

The button itself indicates the selected option. You can include additional controls in the set of options, such as a button to customize the list of options.

To apply this style to a picker, or to a view that contains pickers, use the pickerStyle(_:) modifier.

### Creating the picker style

- init()

## Topics

### Initializers

init()

Creates a pop-up button picker style.

## Relationships

### Conforms To

- PickerStyle

