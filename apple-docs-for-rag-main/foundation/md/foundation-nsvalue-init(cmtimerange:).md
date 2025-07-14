

- Foundation
- NSValue
-  init(CMTimeRange:) 

Initializer

# init(CMTimeRange:)

Creates a new value object containing the specified CoreMedia time range structure.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(CMTimeRange timeRange: CMTimeRange)
```

``` source
init(timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The value for the new object.

## Return Value

A new value object that contains the time range information.

## See Also

### Related Documentation

struct CMTimeRange

A structure that represents a time range.

### Working with Media Time Values

init(CMTime: CMTime)

Creates a new value object containing the specified CoreMedia time structure.

init(CMTimeMapping: CMTimeMapping)

Creates a new value object containing the specified CoreMedia time mapping structure.

var timeValue: CMTime

The CoreMedia time structure representation of the value.

var timeRangeValue: CMTimeRange

The CoreMedia time range structure representation of the value.

var timeMappingValue: CMTimeMapping

The CoreMedia time mapping structure representation of the value.

