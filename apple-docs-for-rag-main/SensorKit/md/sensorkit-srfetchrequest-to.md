

- SensorKit
- SRFetchRequest
-  to 

Instance Property

# to

Fetches sample information that occurs before this time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var to: SRAbsoluteTime { get set }
```

## Discussion

The framework requires the app to define a value for this property. If an app fails to define this property, the framework responds to the fetch by providing SRError.Code.fetchRequestInvalid to the reader delegate via sensorReader(_:fetching:failedWithError:).

## See Also

### Defining the Time Range

var from: SRAbsoluteTime

Fetches sample information that occurs after this time.

struct SRAbsoluteTime

A value that describes when the system records the data.

static func current() -> SRAbsoluteTime

Provides the current absolute time.

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

