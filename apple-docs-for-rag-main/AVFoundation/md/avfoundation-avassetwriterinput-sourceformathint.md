

- AVFoundation
- AVAssetWriterInput
-  sourceFormatHint 

Instance Property

# sourceFormatHint

A hint about the format of the sample buffers to append to the input.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var sourceFormatHint: CMFormatDescription? { get }
```

## Discussion

An input may use this hint to fill in missing output settings or perform additional upfront validation of samples.

Note

To ensure successful file writing when you initialize an input with a source format hint, only append samples of this type.

## See Also

### Inspecting an Input

var mediaType: AVMediaType

The media type of the samples that the input accepts.

var outputSettings: [String : Any]?

The settings to use for encoding media data you append to the output.

