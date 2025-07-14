

- SwiftUI
-  TouchBar 

Structure

# TouchBar

A container for a view that you can show in the Touch Bar.

macOS 10.15+

``` source
struct TouchBar where Content : View
```

## Topics

### Creating a Touch Bar view

init(content: () -> Content)

Creates a non-customizable Touch Bar view container.

init(id: String, content: () -> Content)

Creates a customizable Touch Bar view container with a globally unique identifier.

## See Also

### Managing Touch Bar input

func touchBar&lt;Content>(content: () -> Content) -> some View

Sets the content that the Touch Bar displays.

func touchBar&lt;Content>(TouchBar&lt;Content>) -> some View

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

func touchBarItemPrincipal(Bool) -> some View

Sets principal views that have special significance to this Touch Bar.

func touchBarCustomizationLabel(Text) -> some View

Sets a user-visible string that identifies the view’s functionality.

func touchBarItemPresence(TouchBarItemPresence) -> some View

Sets the behavior of the user-customized view.

enum TouchBarItemPresence

Options that affect user customization of the Touch Bar.

