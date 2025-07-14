

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.InputSource
-  inputSourceID 

Instance Property

# inputSourceID

An identifier for an input source.

macOS 10.7+

``` source
var inputSourceID: String { get }
```

## Discussion

The identifier is unique among the input sources exposed by particular capture device instance.

## See Also

### Accessing Properties

var localizedName: String

A localized, human-readable name for the input source.

