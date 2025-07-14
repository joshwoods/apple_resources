

- SwiftUI
-  WindowResizability 

Structure

# WindowResizability

The resizability of a window.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
struct WindowResizability
```

## Overview

Use the windowResizability(_:) scene modifier to apply a value of this type to a Scene that you define in your App declaration. The value that you specify indicates the strategy the system uses to place minimum and maximum size restrictions on windows that it creates from that scene.

For example, you can create a window group that people can resize to between 100 and 400 points in both dimensions by applying both a frame with those constraints to the scene’s content, and the contentSize resizability to the scene:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
                .frame(
                    minWidth: 100, maxWidth: 400,
                    minHeight: 100, maxHeight: 400)
        }
        .windowResizability(.contentSize)
    }
}
```

The default value for all scenes if you don’t apply the modifier is automatic. With that strategy, Settings windows use the contentSize strategy, while all others use contentMinSize. Windows on visionOS with a window style of volumetric also use the contentSize strategy.

## Topics

### Getting the resizability

static var automatic: WindowResizability

The automatic window resizability.

static var contentMinSize: WindowResizability

A window resizability that’s partially derived from the window’s content.

static var contentSize: WindowResizability

A window resizability that’s derived from the window’s content.

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

func windowIdealSize(WindowIdealSize) -> some Scene

Specifies how windows derived form this scene should determine their size when zooming.

struct WindowIdealSize

A type which defines the size a window should use when zooming.

