

- AVFoundation
- AVAssetWriter
-  canAdd(\_:) 

Instance Method

# canAdd(\_:)

Determines whether the asset writer supports adding the input.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func canAdd(_ input: AVAssetWriterInput) -> Bool
```

## Parameters 

`input`  

The asset writer input to add.

## Return Value

true if you can add the input to the asset writer; otherwise false.

## See Also

### Configuring Inputs

var inputs: [AVAssetWriterInput]

The inputs an asset writer contains.

var availableMediaTypes: [AVMediaType]

The media types the asset writer supports adding as inputs.

func canApply(outputSettings: [String : Any]?, forMediaType: AVMediaType) -> Bool

Determines whether the output file format supports the output settings for a specific media type.

func add(AVAssetWriterInput)

Adds an input to an asset writer.

