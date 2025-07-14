

- SensorKit
- SRAbsoluteTime
-  current() 

Type Method

# current()

Provides the current absolute time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static func current() -> SRAbsoluteTime
```

## Return Value

The absolute time of the current device.

## Discussion

Each device has their own absolute time. This function returns the absolute time of the current device.

## See Also

### Defining the Time Range

var from: SRAbsoluteTime

Fetches sample information that occurs after this time.

var to: SRAbsoluteTime

Fetches sample information that occurs before this time.

struct SRAbsoluteTime

A value that describes when the system records the data.

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

