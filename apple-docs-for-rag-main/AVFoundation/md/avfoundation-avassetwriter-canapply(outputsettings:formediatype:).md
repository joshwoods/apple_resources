

- AVFoundation
- AVAssetWriter
-  canApply(outputSettings:forMediaType:) 

Instance Method

# canApply(outputSettings:forMediaType:)

Determines whether the output file format supports the output settings for a specific media type.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func canApply(
    outputSettings: [String : Any]?,
    forMediaType mediaType: AVMediaType
) -> Bool
```

## Parameters 

`outputSettings`  

The output settings to validate.

`mediaType`  

The media type to validate the output settings for.

## Return Value

true if the format supports the output settings; otherwise, false.

## Discussion

Use this method to determine the compatibility of output settings for a particular media type. For example, video compression settings that specify H.264 compression aren’t compatible with file formats that don’t contain H.264-compressed video.

## See Also

### Configuring Inputs

var inputs: [AVAssetWriterInput]

The inputs an asset writer contains.

var availableMediaTypes: [AVMediaType]

The media types the asset writer supports adding as inputs.

func canAdd(AVAssetWriterInput) -> Bool

Determines whether the asset writer supports adding the input.

func add(AVAssetWriterInput)

Adds an input to an asset writer.

