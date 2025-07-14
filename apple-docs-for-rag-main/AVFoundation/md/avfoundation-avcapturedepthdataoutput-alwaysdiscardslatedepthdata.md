

- AVFoundation
- AVCaptureDepthDataOutput
-  alwaysDiscardsLateDepthData 

Instance Property

# alwaysDiscardsLateDepthData

A Boolean value that determines whether the capture output should discard any depth data that is not processed before the next depth data is captured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var alwaysDiscardsLateDepthData: Bool { get set }
```

## Discussion

If the delegateCallbackQueue dispatch queue is blocked when new depth data is captured, this property determines whether the capture output allows your delegate object more time to process old depth data. If this property’s value is false, the capture output delivers old data to your delegate as soon as possible, but application memory usage may increase as a result. The default value is true.

## See Also

### Configuring Depth Data Capture

var isFilteringEnabled: Bool

A Boolean value that determines whether the depth data output should filter depth data to smooth out noise and fill invalid values.

