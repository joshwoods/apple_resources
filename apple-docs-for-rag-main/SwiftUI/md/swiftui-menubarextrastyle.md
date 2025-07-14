

- SwiftUI
-  MenuBarExtraStyle 

Protocol

# MenuBarExtraStyle

A specification for the appearance and behavior of a menu bar extra scene.

macOS 13.0+

``` source
protocol MenuBarExtraStyle
```

## Topics

### Getting menu bar extra styles

static var automatic: AutomaticMenuBarExtraStyle

The default menu bar extra style.

static var menu: PullDownMenuBarExtraStyle

A menu bar extra style that renders its contents as a menu that pulls down from the icon in the menu bar.

static var window: WindowMenuBarExtraStyle

A menu bar extra style that renders its contents in a popover-like window.

### Supporting types

struct AutomaticMenuBarExtraStyle

The default menu bar extra style. You can also use automatic to construct this style.

struct PullDownMenuBarExtraStyle

A menu bar extra style that renders its contents as a menu that pulls down from the icon in the menu bar.

struct WindowMenuBarExtraStyle

A menu bar extra style that renders its contents in a popover-like window.

## Relationships

### Conforming Types

- AutomaticMenuBarExtraStyle
- PullDownMenuBarExtraStyle
- WindowMenuBarExtraStyle

## See Also

### Creating a menu bar extra

struct MenuBarExtra

A scene that renders itself as a persistent control in the system menu bar.

func menuBarExtraStyle&lt;S>(S) -> some Scene

Sets the style for menu bar extra created by this scene.

