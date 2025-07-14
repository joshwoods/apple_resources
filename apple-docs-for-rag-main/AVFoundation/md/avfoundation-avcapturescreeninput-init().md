

- AVFoundation
- AVCaptureScreenInput
-  init() 

Initializer

# init()

Initializes a capture screen input that provides media data from the main screen.

macOS 10.7+

``` source
init()
```

## Discussion

Using this initializer is equivalent to calling init(displayID:) with the result of the CGMainDisplayID() function.

## See Also

### Initializing a Capture Screen Input

init?(displayID: CGDirectDisplayID)

Initializes a capture screen input that provides media data from the specified display.

