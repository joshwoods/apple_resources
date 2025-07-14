

- AVFoundation
- AVCaptureDataOutputSynchronizer
-  dataOutputs 

Instance Property

# dataOutputs

The list of data outputs governed by this data output synchronizer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var dataOutputs: [AVCaptureOutput] { get }
```

## Discussion

This array is read-only. You configure the list of data outputs to synchronize only when you create an AVCaptureDataOutputSynchronizer object.

Note

The AVCaptureDataOutputSynchronizer class overrides the delegate (and delegate dispatch queue) settings of all of its data outputs, but video and depth data outputs still honor their alwaysDiscardsLateVideoFrames and alwaysDiscardsLateDepthData properties.

## See Also

### Configuring Synchronized Capture

init(dataOutputs: [AVCaptureOutput])

Creates a capture output synchronizer for the specified capture outputs.

