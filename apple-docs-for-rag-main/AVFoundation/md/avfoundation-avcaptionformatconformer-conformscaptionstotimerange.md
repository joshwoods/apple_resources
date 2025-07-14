

- AVFoundation
- AVCaptionFormatConformer
-  conformsCaptionsToTimeRange 

Instance Property

# conformsCaptionsToTimeRange

A Boolean value that indicates whether to conform the time range of a canonical caption.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var conformsCaptionsToTimeRange: Bool { get set }
```

## Discussion

By default, this property value is false. If you set the value to true, this object conforms the time range of captions to fit its encoded data.

When this object conforms captions to CAE608 format, it encodes them so that each CAE608 2-byte control code fits into one frame duration (1001/30000).

## See Also

### Conforming Captions

func conformedCaption(for: AVCaption) throws -> AVCaption

Creates a caption that conforms to a specific format.

