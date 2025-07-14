

- SwiftUI
-  TextFieldLink 

Structure

# TextFieldLink

A control that requests text input from the user when pressed.

watchOS 9.0+

``` source
struct TextFieldLink where Label : View
```

## Overview

A `TextFieldLink` should be used to request text input from the user through a button interface.

## Topics

### Creating a text field link

init(_:prompt:onSubmit:)

Creates a TextFieldLink which when pressed will request text input from the user.

init(prompt: Text?, label: () -> Label, onSubmit: (String) -> Void)

Creates a TextFieldLink which when pressed will request text input from the user.

## Relationships

### Conforms To

- View

## See Also

### Linking to other content

struct Link

A control for navigating to a URL.

struct ShareLink

A view that controls a sharing presentation.

struct SharePreview

A representation of a type to display in a share preview.

struct HelpLink

A button with a standard appearance that opens app-specific help documentation.

