

- Core Motion
- CMTremorResult
-  percentUnknown 

Instance Property

# percentUnknown

The percentage of time when the algorithm couldn’t make a determination.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 5.0+

``` source
var percentUnknown: Float { get }
```

## Discussion

Both active motion and low signal level can cause `percentUnknown` results.

## See Also

### Accessing Tremor Data

var percentNone: Float

The percentage of time when no tremor was detected.

var percentSlight: Float

The percentage of time when a tremor was likely, and the displacement amplitude was slight.

var percentMild: Float

The percentage of time when a tremor was likely, and the displacement amplitude was mild.

var percentModerate: Float

The percentage of time when a tremor was likely, and the displacement amplitude was moderate.

var percentStrong: Float

The percentage of time when a tremor was likely, and the displacement amplitude was strong.

