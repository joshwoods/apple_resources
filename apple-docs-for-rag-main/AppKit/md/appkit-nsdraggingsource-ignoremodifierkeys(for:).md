

- AppKit
- NSDraggingSource
-  ignoreModifierKeys(for:) 

Instance Method

# ignoreModifierKeys(for:)

Returns whether the modifier keys will be ignored for this dragging session.

macOS 10.7+

``` source
@MainActor
optional func ignoreModifierKeys(for session: NSDraggingSession) -> Bool
```

## Parameters 

`session`  

The dragging session.

## Return Value

true if the modifier keys will be ignored, false otherwise.

