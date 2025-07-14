

- Metal
- MTLCaptureManager
-  defaultCaptureScope 

Instance Property

# defaultCaptureScope

The capture scope to use when a capture is initiated in Xcode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var defaultCaptureScope: (any MTLCaptureScope)? { get set }
```

## Discussion

Use this property to specify a default capture scope for Xcode to use when the user presses the capture button. You can still long-press the button to select a different capture scope.

The default value is `nil.` When the value is `nil`, the capture scope is defined by drawable presentation boundaries; such as those created by calls to present(_:) or present().

## See Also

### Creating a Capture Scope

func makeCaptureScope(device: any MTLDevice) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific device object.

func makeCaptureScope(commandQueue: any MTLCommandQueue) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific command queue.

