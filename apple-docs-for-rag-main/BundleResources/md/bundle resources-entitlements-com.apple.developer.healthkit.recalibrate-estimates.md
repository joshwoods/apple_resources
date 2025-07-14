

- Bundle Resources
- Entitlements
-  com.apple.developer.healthkit.recalibrate-estimates 

Property List Key

# com.apple.developer.healthkit.recalibrate-estimates

A Boolean value that determines whether your app can recalibrate the prediction algorithm used to calculate supported sample types.

iOS 15.0+iPadOS 15.0+

## Details 

Type  

boolean

## Discussion

Apps can recalibrate HealthKitʼs prediction algorithms after an event that may significantly affect their results. For example, you can recalibrate the sixMinuteWalkTestDistance type to use only data collected after a mobility-impacting health event, such as surgery or an injury.

To check whether a sample type supports recalibration, see allowsRecalibrationForEstimates. To recalibrate the sample, see recalibrateEstimates(sampleType:date:completion:).

## See Also

### Health

HealthKit Entitlement

A Boolean value that indicates whether the app may request user authorization to access health and activity data that appears in the Health app.

**Key:** com.apple.developer.healthkit

HealthKit Capabilities Entitlement

Health data types that require additional permission.

**Key:** com.apple.developer.healthkit.access

com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

