

- Metal
- MTLCaptureDescriptor
-  destination 

Instance Property

# destination

The destination for any captured command data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var destination: MTLCaptureDestination { get set }
```

## Discussion

The default value is MTLCaptureDestination.developerTools.

## See Also

### Setting Capture Parameters

var captureObject: Any?

The object whose contents should be captured.

var outputURL: URL?

A URL for a file to write the capture data into.

