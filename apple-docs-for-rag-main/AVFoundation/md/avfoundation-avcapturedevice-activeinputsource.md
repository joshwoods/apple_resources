

- AVFoundation
- AVCaptureDevice
-  activeInputSource 

Instance Property

# activeInputSource

The currently active input source of the device.

macOS 10.7+

``` source
var activeInputSource: AVCaptureDevice.InputSource? { get set }
```

## Discussion

You must call lockForConfiguration() before attempting to set a format. Setting a format that isn’t present in the inputSources array results in an exception.

This property is key-value observable.

## See Also

### Configuring Input Sources

var inputSources: [AVCaptureDevice.InputSource]

An array of input sources that the device supports.

class InputSource

A distinct input source on a capture device.

