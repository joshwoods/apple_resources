

- RoomPlan
- RoomCaptureView
-  init(frame:) 

Initializer

# init(frame:)

Creates a view that sizes to the specified frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @preconcurrency
override dynamic init(frame: CGRect)
```

## Parameters 

`frame`  

A structure that positions and shapes the view.

## Overview

This property inherits from UIView.

The system invokes this initializer if you omit the `arSession` argument to init(frame:arSession:). RoomPlan creates its own `ARSession` instance, which you can access through the captureSession property’s arSession.

## See Also

### Creating a room-capture view

init(frame: CGRect, arSession: ARSession)

Creates a room-capture view with the given AR session.

init?(coder: NSCoder)

Creates a view by deserializing from the specified coder.

