

- SwiftUI
-  WindowStyle 

Protocol

# WindowStyle

A specification for the appearance and interaction of a window.

macOS 11.0+visionOS 1.0+

``` source
protocol WindowStyle
```

## Topics

### Getting built-in window styles

static var automatic: DefaultWindowStyle

The default window style.

static var hiddenTitleBar: HiddenTitleBarWindowStyle

A window style which hides both the window’s title and the backing of the titlebar area, allowing more of the window’s content to show.

static var plain: PlainWindowStyle

The plain window style.

static var titleBar: TitleBarWindowStyle

A window style which displays the title bar section of the window.

static var volumetric: VolumetricWindowStyle

A window style that creates a 3D volumetric window.

### Supporting types

struct DefaultWindowStyle

The default window style.

struct HiddenTitleBarWindowStyle

A window style which hides both the window’s title and the backing of the titlebar area, allowing more of the window’s content to show.

struct PlainWindowStyle

The plain window style.

struct TitleBarWindowStyle

A window style which displays the title bar section of the window.

struct VolumetricWindowStyle

A window style that creates a 3D volumetric window.

## Relationships

### Conforming Types

- DefaultWindowStyle
- HiddenTitleBarWindowStyle
- PlainWindowStyle
- TitleBarWindowStyle
- VolumetricWindowStyle

## See Also

### Creating windows

struct WindowGroup

A scene that presents a group of identically structured windows.

struct Window

A scene that presents its content in a single, unique window.

struct UtilityWindow

A specialized window scene that provides secondary utility to the content of the main scenes of an application.

func windowStyle&lt;S>(S) -> some Scene

Sets the style for windows created by this scene.

