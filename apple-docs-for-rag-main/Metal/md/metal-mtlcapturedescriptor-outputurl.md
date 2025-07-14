

- Metal
- MTLCaptureDescriptor
-  outputURL 

Instance Property

# outputURL

A URL for a file to write the capture data into.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var outputURL: URL? { get set }
```

## Discussion

The default value is `nil`. If you set destination to MTLCaptureDestination.gpuTraceDocument, you must set this property to where you want the file to be written to.

## See Also

### Setting Capture Parameters

var captureObject: Any?

The object whose contents should be captured.

var destination: MTLCaptureDestination

The destination for any captured command data.

