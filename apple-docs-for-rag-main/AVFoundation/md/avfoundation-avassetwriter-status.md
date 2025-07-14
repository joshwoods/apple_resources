

- AVFoundation
- AVAssetWriter
-  status 

Instance Property

# status

The status of writing samples to the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var status: AVAssetWriter.Status { get }
```

## Discussion

This property is thread safe.

## See Also

### Inspecting Writing Status

enum Status

Values that indicate the state of an asset writer.

var error: (any Error)?

An error object that describes an asset-writing failure.

