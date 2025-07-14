

- Exposure Notification
- ENExposureConfiguration
-  otherDurationWeight 

Instance Property

# otherDurationWeight

The weight assigned to a risk level indicating the duration of the user’s exposure at a large distance.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var otherDurationWeight: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

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

var daysSinceLastExposureThreshold: Int

The number of days to consider when calculating the risk level.

