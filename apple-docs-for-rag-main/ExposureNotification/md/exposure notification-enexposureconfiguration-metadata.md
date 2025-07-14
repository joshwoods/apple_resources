

- Exposure Notification
- ENExposureConfiguration
-  metadata 

Instance Property

# metadata

The metadata you use to configure the exposure calculations.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var metadata: [AnyHashable : Any]? { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

Not used.

## See Also

### Level Configuration

var attenuationDurationThresholds: [NSNumber]

The configurable signal-loss thresholds for calculating exposure risk.

var attenuationLevelValues: [NSNumber]

The level values for attenuation.

var daysSinceLastExposureLevelValues: [NSNumber]

The level values for days since last exposure.

var durationLevelValues: [NSNumber]

The level values for duration.

var transmissionRiskLevelValues: [NSNumber]

The level values for transmission risk.

