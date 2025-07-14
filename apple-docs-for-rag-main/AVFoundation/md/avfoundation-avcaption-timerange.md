

- AVFoundation
- AVCaption
-  timeRange 

Instance Property

# timeRange

The time range over which the system presents the caption.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var timeRange: CMTimeRange { get }
```

## Discussion

Apple iTT format only permits captions to have overlapping time ranges if they’re associated with different regions.

CEA608 closed caption time ranges can’t start with zero, because the decoder needs transmission time. Align time ranges with the video frame rate.

## See Also

### Accessing Text and Timing

var text: String

The caption text.

