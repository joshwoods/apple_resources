

- SwiftUI
-  DefaultToggleStyle 

Structure

# DefaultToggleStyle

The default toggle style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct DefaultToggleStyle
```

## Overview

Use the automatic static variable to create this style:

```
Toggle("Enhance Sound", isOn: $isEnhanced)
    .toggleStyle(.automatic)
```

## Topics

### Creating the toggle style

init()

Creates a default toggle style.

### Supporting types

func makeBody(configuration: DefaultToggleStyle.Configuration) -> some View

Creates a view that represents the body of a toggle.

## Relationships

### Conforms To

- ToggleStyle

## See Also

### Supporting types

struct ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

struct CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

struct SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

