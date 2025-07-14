

- AVKit
- AVCaptureEventInteraction
-  init(primary:secondary:) 

Initializer

# init(primary:secondary:)

Creates a capture event interaction with handlers that respond independently to presses of hardware buttons.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
@MainActor
init(
    primary primaryHandler: @escaping (AVCaptureEvent) -> Void,
    secondary secondaryHandler: @escaping (AVCaptureEvent) -> Void
)
```

## Parameters 

`primaryHandler`  

An event handler the system calls when a person performs a primary capture event.

`secondaryHandler`  

An event handler the system calls when a person performs a secondary capture event.

## See Also

### Creating an interaction

init(handler: (AVCaptureEvent) -> Void)

Creates a capture event interaction with a handler that responds to presses of hardware buttons.

