

- Exposure Notification
- ENExposureConfiguration
-  Exposure Risk Value Calculation in ExposureNotification Version 1 

API Collection

# Exposure Risk Value Calculation in ExposureNotification Version 1

Learn how to determine a user’s risk of exposure.

## Overview

The ExposureNotification framework uses an Exposure Risk Value to assist the user in determining whether they may have been exposed to the coronavirus. Health authorities have flexibility in calculating this value by setting weights and values in a configuration object.

To adopt this method of risk assessment, set the `ENAPIVersion` key to the integer value `1` in the app’s `Info.plist`.

The following diagram illustrates the data structure and formula used to calculate the Exposure Risk Value.

The following parameters are used to calculate a risk for each exposure incident:

Transmission Risk  
Transmission risk is intended to reflect the status of infection in the affected user and its effect on risk of transmission. The value is based on the affected user’s symptoms, when symptoms first appeared, level of diagnosis verification, or other determination from the app or a health authority.

Duration  
Cumulative duration of the exposure. The framework measures this value.

Days  
Days since the exposure incident. The framework measures this value.

Attenuation  
The attenuation (`transmission power - RSSI`) can vary during an exposure event. Attenuation values greater than 0 are weighted by the duration at each risk level and averaged for the overall duration. The framework measures and calculates this value.

The totalRiskScore is calculated using the following formula:

```
totalRiskScore = transmissionRiskValue * durationRiskValue *
daysSinceLastExposureRiskValue * attenuationRiskValue
```

Level values are in the range of 0-8. While the formula’s range can be up to 4096, the framework limits totalRiskScore to the upper limit of ENRiskScore, which has a maximum value of 255.

The following diagram illustrates an example of an Exposure Risk Value calculated for a person who was exposed to another person who was diagnosed positive.

For this example, the other user reported a positive diagnosis, the encounter between the two devices lasted 14 minutes, it happened 4 days ago, and the signal strength attenuation between their phones had a weighted average of 68. The `totalRiskScore` is limited and set to 255.

To exclude exposure incidents with a risk score below a certain amount, set  minimumRiskScoreFullRange. The framework doesn’t use this property when calculating matchedKeyCount or daysSinceLastExposureThreshold.

## Topics

### Exposure Information

class ENExposureInfo

The incident information related to a potential exposure.

typealias ENRiskScore

A value signifying the risk of an exposure event.

typealias ENRiskLevel

The user’s estimated risk of exposure.

typealias ENRiskLevelValue

The value associated with a particular risk level.

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

var metadata: [AnyHashable : Any]?

The metadata you use to configure the exposure calculations.

### Minimum Threshold Configuration

var minimumRiskScore: ENRiskScore

The value that is the user’s minimum risk score.

var minimumRiskScoreFullRange: Double

The value that is the user’s full-range minimum risk score.

### Weight Configuration

var attenuationWeight: Double

The weight assigned to a score for the Bluetooth signal strength.

var daysSinceLastExposureWeight: Double

The weight assigned to a score for the days since the user’s exposure.

var durationWeight: Double

The weight assigned to a score for the duration of the user’s exposure.

var transmissionRiskWeight: Double

The weight assigned to a score for the affected user’s estimated risk of transmission.

