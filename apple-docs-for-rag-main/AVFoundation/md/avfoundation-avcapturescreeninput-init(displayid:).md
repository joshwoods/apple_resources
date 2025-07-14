

- AVFoundation
- AVCaptureScreenInput
-  init(displayID:) 

Initializer

# init(displayID:)

Initializes a capture screen input that provides media data from the specified display.

macOS 10.7+

``` source
init?(displayID: CGDirectDisplayID)
```

## Parameters 

`displayID`  

The ID of the display from which to capture video.

`CGDirectDisplayID` is defined in ``.

## Return Value

A capture screen input initialized to provide media data from a given display. If the display cannot be used (because it is not available on the system, for example), returns `nil`.

## See Also

### Initializing a Capture Screen Input

init()

Initializes a capture screen input that provides media data from the main screen.

