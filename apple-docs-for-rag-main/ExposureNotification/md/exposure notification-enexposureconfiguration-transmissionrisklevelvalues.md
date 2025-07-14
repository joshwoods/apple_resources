

- Exposure Notification
- ENExposureConfiguration
-  transmissionRiskLevelValues 

Instance Property

# transmissionRiskLevelValues

The level values for transmission risk.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var transmissionRiskLevelValues: [NSNumber] { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

This property contains eight levels, one for each type of transmission risk:

- `transmissionRiskScores[0]` for risk level 0.

- `transmissionRiskScores[1]` for risk level 1.

- `transmissionRiskScores[2]` for risk level 2.

- `transmissionRiskScores[3]` for risk level 3.

- `transmissionRiskScores[4]` for risk level 4.

- `transmissionRiskScores[5]` for risk level 5.

- `transmissionRiskScores[6]` for risk level 6.

- `transmissionRiskScores[7]` for risk level 7.

Each app defines its own meaning for each of the risk levels (0-7). The values assigned to each risk level should be in the range of 0-8.

Consistent Transmission Risk Levels across regions facilitate roaming, therefore it’s recommended that the Transmission Risk Levels describe the type of report. The supported report types are determined by the public health authority for each region. Your app must verify the report type with a public health authority before submitting it.

Recommended report types for the different risk levels are:

- `0` = Unused/Custom

- `1` = Confirmed test: Low transmission risk level

- `2` = Confirmed test: Standard transmission risk level

- `3` = Confirmed test: High transmission risk level

- `4` = Confirmed clinical diagnosis

- `5` = Self report

- `6` = Negative case

- `7` = Recursive case

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

var metadata: [AnyHashable : Any]?

The metadata you use to configure the exposure calculations.

