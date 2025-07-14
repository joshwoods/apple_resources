

- AVFoundation
- AVAssetWriterInputCaptionAdaptor
-  append(\_:) 

Instance Method

# append(\_:)

Appends a caption to the writer input.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func append(_ caption: AVCaption) -> Bool
```

## Parameters 

`caption`  

The caption that the system appends to the writer input.

## Return Value

A Boolean value that indicates whether the operation succeeded.

## See Also

### Appending Captions

func append(AVCaptionGroup) -> Bool

Appends a caption group that the system writes to the output.

