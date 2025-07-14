

- SwiftUI
-  ButtonToggleStyle 

Structure

# ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 9.0+

``` source
struct ButtonToggleStyle
```

## Overview

You can also use button to construct this style.

```
Toggle(isOn: $isFlagged) {
    Label("Flag", systemImage: "flag.fill")
}
.toggleStyle(.button)
```

## Topics

### Creating the toggle style

init()

Creates a button toggle style.

### Supporting types

func makeBody(configuration: ButtonToggleStyle.Configuration) -> some View

Creates a view that represents the body of a toggle button.

## Relationships

### Conforms To

- ToggleStyle

## See Also

### Supporting types

struct DefaultToggleStyle

The default toggle style.

struct CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

struct SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

