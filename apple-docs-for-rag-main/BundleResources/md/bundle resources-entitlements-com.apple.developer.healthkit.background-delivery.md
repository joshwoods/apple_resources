

- Bundle Resources
- Entitlements
-  com.apple.developer.healthkit.background-delivery 

Property List Key

# com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

iOS 15.0+iPadOS 15.0+visionOS 1.0+watchOS 8.0+

## Details 

Type  

boolean

## Discussion

If this key is true, your app can enable background delivery of HKObserverQuery instances by calling the HealthKit store’s enableBackgroundDelivery(for:frequency:withCompletion:) method. By default, the value is false.

## See Also

### Health

HealthKit Entitlement

A Boolean value that indicates whether the app may request user authorization to access health and activity data that appears in the Health app.

**Key:** com.apple.developer.healthkit

HealthKit Capabilities Entitlement

Health data types that require additional permission.

**Key:** com.apple.developer.healthkit.access

com.apple.developer.healthkit.recalibrate-estimates

A Boolean value that determines whether your app can recalibrate the prediction algorithm used to calculate supported sample types.

