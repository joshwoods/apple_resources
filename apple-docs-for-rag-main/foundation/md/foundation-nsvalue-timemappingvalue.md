

- Foundation
- NSValue
-  timeMappingValue 

Instance Property

# timeMappingValue

The CoreMedia time mapping structure representation of the value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var timeMappingValue: CMTimeMapping { get }
```

## See Also

### Related Documentation

struct CMTimeMapping

A structure that maps a segment of a source time range to a target time range.

### Working with Media Time Values

init(CMTime: CMTime)

Creates a new value object containing the specified CoreMedia time structure.

init(CMTimeRange: CMTimeRange)

Creates a new value object containing the specified CoreMedia time range structure.

init(CMTimeMapping: CMTimeMapping)

Creates a new value object containing the specified CoreMedia time mapping structure.

var timeValue: CMTime

The CoreMedia time structure representation of the value.

var timeRangeValue: CMTimeRange

The CoreMedia time range structure representation of the value.

