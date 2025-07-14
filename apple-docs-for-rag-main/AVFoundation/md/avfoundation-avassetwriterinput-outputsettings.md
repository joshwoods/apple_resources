

- AVFoundation
- AVAssetWriterInput
-  outputSettings 

Instance Property

# outputSettings

The settings to use for encoding media data you append to the output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var outputSettings: [String : Any]? { get }
```

## Discussion

A value of `nil` indicates that the input passes the samples through to the output without reencoding them.

## See Also

### Inspecting an Input

var mediaType: AVMediaType

The media type of the samples that the input accepts.

var sourceFormatHint: CMFormatDescription?

A hint about the format of the sample buffers to append to the input.

