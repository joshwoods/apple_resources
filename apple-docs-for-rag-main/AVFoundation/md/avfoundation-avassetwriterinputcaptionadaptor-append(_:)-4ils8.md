

- AVFoundation
- AVAssetWriterInputCaptionAdaptor
-  append(\_:) 

Instance Method

# append(\_:)

Appends a caption group that the system writes to the output.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func append(_ captionGroup: AVCaptionGroup) -> Bool
```

## Parameters 

`captionGroup`  

The caption group that the system writes to the output.

## Return Value

A Boolean value that indicates whether the operation succeeded.

## See Also

### Appending Captions

func append(AVCaption) -> Bool

Appends a caption to the writer input.

