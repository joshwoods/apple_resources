

- RoomPlan
- RoomCaptureView
-  init(coder:) 

Initializer

# init(coder:)

Creates a view by deserializing from the specified coder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @preconcurrency
required dynamic init?(coder: NSCoder)
```

## Parameters 

`coder`  

An object from which the view deserializes.

## Overview

This property inherits from UIView.

## See Also

### Creating a room-capture view

init(frame: CGRect, arSession: ARSession)

Creates a room-capture view with the given AR session.

init(frame: CGRect)

Creates a view that sizes to the specified frame.

