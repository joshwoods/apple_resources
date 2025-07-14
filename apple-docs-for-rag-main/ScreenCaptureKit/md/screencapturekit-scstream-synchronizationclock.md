

- ScreenCaptureKit
- SCStream
-  synchronizationClock 

Instance Property

# synchronizationClock

A clock to use for output synchronization.

Mac Catalyst 16.1+macOS 13.0+

``` source
var synchronizationClock: CMClock? { get }
```

## Discussion

The synchronization clock provides the timebase for sample buffers that the stream outputs. Use it to synchronize with the clocks of other media sources, such as the synchronizationClock of AVCaptureSession.

