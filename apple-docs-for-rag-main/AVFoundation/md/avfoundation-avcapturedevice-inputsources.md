

- AVFoundation
- AVCaptureDevice
-  inputSources 

Instance Property

# inputSources

An array of input sources that the device supports.

macOS 10.7+

``` source
var inputSources: [AVCaptureDevice.InputSource] { get }
```

## Discussion

Some devices can capture data from one of multiple data sources (different input jacks on the same audio device, for example). For devices with multiple possible data sources, you can use this property to enumerate the possible choices.

This value is key-value observable.

## See Also

### Configuring Input Sources

var activeInputSource: AVCaptureDevice.InputSource?

The currently active input source of the device.

class InputSource

A distinct input source on a capture device.

