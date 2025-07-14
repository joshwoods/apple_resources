

- AVFoundation
- AVAssetWriter
-  error 

Instance Property

# error

An error object that describes an asset-writing failure.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var error: (any Error)? { get }
```

## See Also

### Inspecting Writing Status

var status: AVAssetWriter.Status

The status of writing samples to the output file.

enum Status

Values that indicate the state of an asset writer.

