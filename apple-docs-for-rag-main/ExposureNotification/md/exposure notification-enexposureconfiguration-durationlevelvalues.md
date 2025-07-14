

- Exposure Notification
- ENExposureConfiguration
-  durationLevelValues 

Instance Property

# durationLevelValues

The level values for duration.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var durationLevelValues: [NSNumber] { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

This property contains eight levels, each defining a range of exposure duration:

- `durationScores[0]` when duration equals 0.

- `durationScores[1]` when duration \ 30.

## See Also

### Level Configuration

var attenuationDurationThresholds: [NSNumber]

The configurable signal-loss thresholds for calculating exposure risk.

var attenuationLevelValues: [NSNumber]

The level values for attenuation.

var daysSinceLastExposureLevelValues: [NSNumber]

The level values for days since last exposure.

var transmissionRiskLevelValues: [NSNumber]

The level values for transmission risk.

var metadata: [AnyHashable : Any]?

The metadata you use to configure the exposure calculations.

