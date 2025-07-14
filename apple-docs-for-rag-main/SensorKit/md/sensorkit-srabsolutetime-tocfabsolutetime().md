

- SensorKit
- SRAbsoluteTime
-  toCFAbsoluteTime() 

Instance Method

# toCFAbsoluteTime()

Converts an absolute time to a core-foundation absolute time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func toCFAbsoluteTime() -> CFAbsoluteTime
```

## Return Value

The core-foundation absolute time.

## See Also

### Defining the Time Range

var from: SRAbsoluteTime

Fetches sample information that occurs after this time.

var to: SRAbsoluteTime

Fetches sample information that occurs before this time.

struct SRAbsoluteTime

A value that describes when the system records the data.

static func current() -> SRAbsoluteTime

Provides the current absolute time.

