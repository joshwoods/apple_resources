

- SwiftUI
-  MenuButton Deprecated

Structure

# MenuButton

A button that displays a menu containing a list of choices when pressed.

macOS 10.15–15.4Deprecated

``` source
struct MenuButton where Label : View, Content : View
```

Deprecated

Use Menu instead.

## Topics

### Creating a menu button

init(_:content:)

Creates a menu button with the specified localized title and content.

init(label: Label, content: () -> Content)

Creates a menu button with the specified label and content.

### Styling a menu button

func menuButtonStyle&lt;S>(S) -> some View

Sets the style for menu buttons within this view.

protocol MenuButtonStyle

A custom specification for the appearance and interaction of a menu button.

## Relationships

### Conforms To

- View

## See Also

### Deprecated types

typealias PullDownButtonDeprecated

struct ContextMenu

A container for views that you present as menu items in a context menu.

Deprecated

