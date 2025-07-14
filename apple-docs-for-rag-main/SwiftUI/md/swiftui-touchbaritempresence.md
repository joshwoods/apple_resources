

- SwiftUI
-  TouchBarItemPresence 

Enumeration

# TouchBarItemPresence

Options that affect user customization of the Touch Bar.

macOS 10.15+

``` source
enum TouchBarItemPresence
```

## Topics

### Getting presence options

case `default`(String)

The Touch Bar view is visible by default, but can be removed during customization.

case optional(String)

The Touch Bar view isn’t visible by default, but appears in the customization palette.

case required(String)

The Touch Bar view is visible by default and cannot be removed during customization.

## Relationships

### Conforms To

- Sendable

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

struct TouchBar

A container for a view that you can show in the Touch Bar.

