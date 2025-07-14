

- AVFoundation
- AVCaptionFormatConformer
-  conformedCaption(for:) 

Instance Method

# conformedCaption(for:)

Creates a caption that conforms to a specific format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func conformedCaption(for caption: AVCaption) throws -> AVCaption
```

## Parameters 

`caption`  

The caption to conform.

## Return Value

A caption that conforms to the defined caption format.

## See Also

### Conforming Captions

var conformsCaptionsToTimeRange: Bool

A Boolean value that indicates whether to conform the time range of a canonical caption.

