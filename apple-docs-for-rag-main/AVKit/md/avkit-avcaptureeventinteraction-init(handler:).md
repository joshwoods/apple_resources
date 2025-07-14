

- AVKit
- AVCaptureEventInteraction
-  init(handler:) 

Initializer

# init(handler:)

Creates a capture event interaction with a handler that responds to presses of hardware buttons.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
@MainActor
init(handler: @escaping (AVCaptureEvent) -> Void)
```

## Parameters 

`handler`  

An event handler the system calls when a person performs a primary or secondary capture event.

## See Also

### Creating an interaction

init(primary: (AVCaptureEvent) -> Void, secondary: (AVCaptureEvent) -> Void)

Creates a capture event interaction with handlers that respond independently to presses of hardware buttons.

