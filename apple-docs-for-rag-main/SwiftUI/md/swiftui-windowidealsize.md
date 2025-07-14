

- SwiftUI
-  WindowIdealSize 

Structure

# WindowIdealSize

A type which defines the size a window should use when zooming.

macOS 15.0+

``` source
struct WindowIdealSize
```

## Overview

Use this type in conjunction with the `Scene.windowIdealSize(_:)` modifier to override the default behavior for how windows behave when performing a zoom.

For example, you can define a window group where the window has an ideal width of 800 points and an ideal height of 600 points:

```
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
                .frame(idealWidth: 800, idealHeight: 600)
        }
        .windowIdealSize(.fitToContent)
    }
}
```

## Topics

### Type Properties

static let automatic: WindowIdealSize

The automatic window ideal size. Windows will use the system behavior when determining the size to use when zooming.

static let fitToContent: WindowIdealSize

A window ideal size which uses the ideal size of the window’s contents.

static let maximum: WindowIdealSize

A window ideal size which uses the maximum size of the window’s contents.

## Relationships

### Conforms To

- Sendable

## See Also

### Sizing a window

Positioning and sizing windows

Influence the initial geometry of windows that your app presents.

func defaultSize(_:)

Sets a default size for a window.

func defaultSize(width: CGFloat, height: CGFloat) -> some Scene

Sets a default width and height for a window.

func defaultSize(width: CGFloat, height: CGFloat, depth: CGFloat) -> some Scene

Sets a default size for a volumetric window.

func defaultSize(Size3D, in: UnitLength) -> some Scene

Sets a default size for a volumetric window.

func defaultSize(width: CGFloat, height: CGFloat, depth: CGFloat, in: UnitLength) -> some Scene

Sets a default size for a volumetric window.

func windowResizability(WindowResizability) -> some Scene

Sets the kind of resizability to use for a window.

struct WindowResizability

The resizability of a window.

func windowIdealSize(WindowIdealSize) -> some Scene

Specifies how windows derived form this scene should determine their size when zooming.

