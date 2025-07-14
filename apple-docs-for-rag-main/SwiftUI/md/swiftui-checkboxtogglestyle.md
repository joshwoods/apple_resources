

- SwiftUI
-  CheckboxToggleStyle 

Structure

# CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

macOS 10.15+

``` source
struct CheckboxToggleStyle
```

## Overview

Use the checkbox static variable to create this style:

```
Toggle("Close windows when quitting an app", isOn: $doesClose)
    .toggleStyle(.checkbox)
```

## Topics

### Creating the toggle style

init()

Creates a checkbox toggle style.

### Supporting types

func makeBody(configuration: CheckboxToggleStyle.Configuration) -> some View

Creates a view that represents the body of a toggle checkbox.

## Relationships

### Conforms To

- ToggleStyle

## See Also

### Supporting types

struct DefaultToggleStyle

The default toggle style.

struct ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

struct SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

