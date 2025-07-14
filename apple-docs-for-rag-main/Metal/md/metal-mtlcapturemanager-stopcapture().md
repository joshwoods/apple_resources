

- Metal
- MTLCaptureManager
-  stopCapture() 

Instance Method

# stopCapture()

Stops capturing Metal commands.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func stopCapture()
```

## Discussion

Calling this method stops a capture that was started manually in Xcode or programmatically by calling one of the methods on MTLCaptureManager.

When using a custom capture scope, calling this function preempts any end() demarcations of the capture scope.

