

- SwiftUI
-  SwitchToggleStyle 

Structure

# SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 18.0+visionOS 1.0+watchOS 6.0+

``` source
struct SwitchToggleStyle
```

## Overview

Use the switch static variable to create this style:

```
Toggle("Enhance Sound", isOn: $isEnhanced)
    .toggleStyle(.switch)
```

## Topics

### Creating the toggle style

init()

Creates a switch toggle style.

### Supporting types

func makeBody(configuration: SwitchToggleStyle.Configuration) -> some View

Creates a view that represents the body of a toggle switch.

### Deprecated initializers

init(tint: Color)

Creates a switch style with a tint color.

Deprecated

## Relationships

### Conforms To

- ToggleStyle

## See Also

### Supporting types

struct DefaultToggleStyle

The default toggle style.

struct ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

struct CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

