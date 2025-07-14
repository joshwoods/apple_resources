

- AVFoundation
- AVAssetWriter
-  inputs 

Instance Property

# inputs

The inputs an asset writer contains.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var inputs: [AVAssetWriterInput] { get }
```

## See Also

### Configuring Inputs

var availableMediaTypes: [AVMediaType]

The media types the asset writer supports adding as inputs.

func canApply(outputSettings: [String : Any]?, forMediaType: AVMediaType) -> Bool

Determines whether the output file format supports the output settings for a specific media type.

func canAdd(AVAssetWriterInput) -> Bool

Determines whether the asset writer supports adding the input.

func add(AVAssetWriterInput)

Adds an input to an asset writer.

