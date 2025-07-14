

- SwiftUI
- WindowPlacement
-  WindowPlacement.Position 

Structure

# WindowPlacement.Position

A semantic or positional value for the location of a window.

visionOS 2.0+

``` source
struct Position
```

## Topics

### Type Properties

static var utilityPanel: WindowPlacement.Position

Utility panel window position.

### Type Methods

static func above(WindowProxy) -> WindowPlacement.Position

Window position relative to the top edge of another window.

static func below(WindowProxy) -> WindowPlacement.Position

Window position relative to the bottom edge of another window.

static func leading(WindowProxy) -> WindowPlacement.Position

Window position relative to the leading edge of another window.

static func replacing(WindowProxy) -> WindowPlacement.Position

Positions the window in the same spot as an existing window, hiding the old window in the process.

Deprecated

static func trailing(WindowProxy) -> WindowPlacement.Position

Window position relative to the trailing edge of another window.

## Relationships

### Conforms To

- Equatable

