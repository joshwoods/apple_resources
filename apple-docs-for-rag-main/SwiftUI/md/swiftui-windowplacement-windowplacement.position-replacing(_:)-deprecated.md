

- SwiftUI
- WindowPlacement
- WindowPlacement.Position
-  replacing(\_:) Deprecated

Type Method

# replacing(\_:)

Positions the window in the same spot as an existing window, hiding the old window in the process.

visionOS 2.0–2.0Deprecated

``` source
static func replacing(_ relativeWindow: WindowProxy) -> WindowPlacement.Position
```

Deprecated

Use PushWindowAction instead.

## Parameters 

`relativeWindow`  

The existing window that the new window will replace.

## Discussion

This will position the new window in the same location as the specified existing window, and hide the old window. Closing the new window will then result in the original window being shown again.

