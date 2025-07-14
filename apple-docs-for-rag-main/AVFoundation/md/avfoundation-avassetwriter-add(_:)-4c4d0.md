

- AVFoundation
- AVAssetWriter
-  add(\_:) 

Instance Method

# add(\_:)

Adds an input to an asset writer.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func add(_ input: AVAssetWriterInput)
```

## Parameters 

`input`  

A compatible asset writer input to add.

## Discussion

You can’t add inputs after asset writing begins.

## See Also

### Configuring Inputs

var inputs: [AVAssetWriterInput]

The inputs an asset writer contains.

var availableMediaTypes: [AVMediaType]

The media types the asset writer supports adding as inputs.

func canApply(outputSettings: [String : Any]?, forMediaType: AVMediaType) -> Bool

Determines whether the output file format supports the output settings for a specific media type.

func canAdd(AVAssetWriterInput) -> Bool

Determines whether the asset writer supports adding the input.

