

- Bundle Resources
- Entitlements
-  HealthKit Capabilities Entitlement 

Property List Key

# HealthKit Capabilities Entitlement

Health data types that require additional permission.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

## Details 

Key  
com.apple.developer.healthkit.access

Type  

array of strings

## Possible Values 

`health-records`  

The app can request access to FHIR-backed clinical records.

## Discussion

The HealthKit Entitlement provides access to most HealthKit data types. However, because of their highly sensitive nature, some data types require additional entitlements. The HealthKit Capabilities Entitlement provides access to these data types.

To add this entitlement to your app, first enable the HealthKit capability in Xcode, and then check any values that you want to add to the HealthKit Capabilities Entitlement.

Only add values for data types that your app needs to access. App Review may reject apps that don’t use the data appropriately. For more information, see the Health and Health Research section of the App Store Review Guidelines.

## See Also

### Related Documentation

Accessing Health Records

Read clinical record data from the HealthKit store.

### Health

HealthKit Entitlement

A Boolean value that indicates whether the app may request user authorization to access health and activity data that appears in the Health app.

**Key:** com.apple.developer.healthkit

com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

com.apple.developer.healthkit.recalibrate-estimates

A Boolean value that determines whether your app can recalibrate the prediction algorithm used to calculate supported sample types.

