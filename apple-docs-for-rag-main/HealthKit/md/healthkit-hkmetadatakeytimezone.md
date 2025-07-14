

- HealthKit
-  HKMetadataKeyTimeZone 

Global Variable

# HKMetadataKeyTimeZone

The user’s time zone when the HealthKit object was created.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyTimeZone: String
```

## Discussion

This key takes a string value compatible with the NSTimeZone class’s timeZoneWithName: method. For best results when analyzing sleep samples, it’s recommended that you store time zone metadata with your sleep sample data.

## See Also

### General Keys

let HKMetadataKeyExternalUUID: String

A unique identifier for an HKObject that is set by its source.

let HKMetadataKeyWasUserEntered: String

A key that indicates whether the sample was entered by the user.

let HKMetadataKeyQuantityClampedToLowerBound: String

let HKMetadataKeyQuantityClampedToUpperBound: String

