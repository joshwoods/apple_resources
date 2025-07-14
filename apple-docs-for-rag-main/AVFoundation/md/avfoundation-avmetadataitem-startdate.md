

- AVFoundation
- AVMetadataItem
-  startDate 

Instance Property

# startDate

The start date of the timed metadata.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var startDate: Date? { get }
```

## Discussion

The value is `nil` if the metadata item doesn’t provide a start date.

## See Also

### Accessing Timing

var time: CMTime

The timestamp of the metadata item.

var duration: CMTime

The duration of the metadata item.

