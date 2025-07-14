

- Exposure Notification
- ENExposureConfiguration
-  daysSinceLastExposureThreshold 

Instance Property

# daysSinceLastExposureThreshold

The number of days to consider when calculating the risk level.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var daysSinceLastExposureThreshold: Int { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

The default value is 0, meaning no filtering is applied.

## See Also

### Configuring Duration

var attenuationDurationThresholds: [NSNumber]

The configurable signal-loss thresholds for calculating exposure risk.

var immediateDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at immediate distance.

var mediumDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at medium distance.

var nearDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at close distance.

var otherDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at a large distance.

