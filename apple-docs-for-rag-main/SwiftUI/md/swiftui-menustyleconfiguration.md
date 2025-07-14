

- SwiftUI
-  MenuStyleConfiguration 

Structure

# MenuStyleConfiguration

A configuration of a menu.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
struct MenuStyleConfiguration
```

## Overview

Use the init(_:) initializer of Menu to create an instance using the current menu style, which you can modify to create a custom style.

For example, the following code creates a new, custom style that adds a red border to the current menu style:

```
struct RedBorderMenuStyle: MenuStyle {
    func makeBody(configuration: Configuration) -> some View {
        Menu(configuration)
            .border(Color.red)
    }
}
```

## Topics

### Setting the label and content

struct Label

A type-erased label of a menu.

struct Content

A type-erased content of a menu.

## See Also

### Styling menus

func menuStyle&lt;S>(S) -> some View

Sets the style for menus within this view.

protocol MenuStyle

A type that applies standard interaction behavior and a custom appearance to all menus within a view hierarchy.

