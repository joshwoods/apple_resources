

- SensorKit
- SRFetchRequest
-  from 

Instance Property

# from

Fetches sample information that occurs after this time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var from: SRAbsoluteTime { get set }
```

## Discussion

A fetch is exclusive of this time.

The framework requires the app to define a value for this property. If an app fails to define this property, the framework responds to the fetch by providing SRError.Code.fetchRequestInvalid to the reader delegate via sensorReader(_:fetching:failedWithError:).

## See Also

### Defining the Time Range

var to: SRAbsoluteTime

Fetches sample information that occurs before this time.

struct SRAbsoluteTime

A value that describes when the system records the data.

static func current() -> SRAbsoluteTime

Provides the current absolute time.

func toCFAbsoluteTime() -> CFAbsoluteTime

Converts an absolute time to a core-foundation absolute time.

