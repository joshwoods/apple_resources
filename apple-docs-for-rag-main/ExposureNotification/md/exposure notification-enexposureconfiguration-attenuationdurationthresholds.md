

- Exposure Notification
- ENExposureConfiguration
-  attenuationDurationThresholds 

Instance Property

# attenuationDurationThresholds

The configurable signal-loss thresholds for calculating exposure risk.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var attenuationDurationThresholds: [NSNumber] { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.6 and later.

Signal attenuation and duration are measurable aspects of exposure risk. Set threshold values to configure the degree to which the signal loss between two devices for a specific duration signifies a potential exposure. Four categories are described in ENExposureConfiguration: *immediate*, *near*, *medium*, and *other*.

The following entries in the `attenuationDurationThresholds` array correspond to three thresholds for the four categories:

`attenuationDurationThresholds[0]`  
The immediate duration threshold. The framework sums the duration of exposures for which the attenuation is less than or equal to `attenuationDurationThresholds[0]`. The default value is `50`.

`attenuationDurationThresholds[1]`  
The near attenuation threshold. The framework sums the duration of exposures for which the attenuation is greater than `attenuationDurationThresholds[0]` and less than or equal to `attenuationDurationThresholds[1]`. The default value is `70`.

`attenuationDurationThresholds[2]`  
The medium attenuation threshold. The framework sums the duration of exposures for which the attenuation is greater than `attenuationDurationThresholds[1]` and less than or equal to `attenuationDurationThresholds[2]`. The default value is `90`.

Attenuation values greater than `attenuationDurationThresholds[2]` accumulate into the “other” category.

## See Also

### Configuring Duration

var immediateDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at immediate distance.

var mediumDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at medium distance.

var nearDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at close distance.

var otherDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at a large distance.

var daysSinceLastExposureThreshold: Int

The number of days to consider when calculating the risk level.

