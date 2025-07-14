

- AVFoundation
- AVCaptureSynchronizedData
-  timestamp 

Instance Property

# timestamp

The time at which this synchronized data was captured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var timestamp: CMTime { get }
```

## Discussion

Synchronized data is always synchronized to the masterClock time of the AVCaptureSession object to which the data output is connected.

