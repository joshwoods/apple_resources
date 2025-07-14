

- AVFoundation
- AVCaptureSession
-  masterClock Deprecated

Instance Property

# masterClock

A clock object used for output synchronization.

iOS 7.0–15.4DeprecatediPadOS 7.0–15.4DeprecatedMac Catalyst 14.0–15.4DeprecatedmacOS 10.9–12.3Deprecated

``` source
var masterClock: CMClock? { get }
```

Deprecated

Use synchronizationClock instead.

## Discussion

The returned CMClock object is read-only and provides a timebase for all sample buffers in capture output. Use this clock in conjunction with the clock from an AVCaptureInput.Port object to synchronize capture output with external data sources such as motion samples.

For example, to synchronize output timestamps to the original timestamps provided by an input device, you can do the following in your fileOutput(_:didOutputSampleBuffer:from:) method:

```
guard let masterClock = captureSession.masterClock,
    let originalClock = connection.inputPorts.first?.clock else { return }

let synchedPTS = sampleBuffer.presentationTimeStamp
let originalPTS = masterClock.convertTime(synchedPTS, to: originalClock)
```

This property is key-value observable.

## See Also

### Synchronizing Output

var synchronizationClock: CMClock?

A clock to use for output synchronization.

