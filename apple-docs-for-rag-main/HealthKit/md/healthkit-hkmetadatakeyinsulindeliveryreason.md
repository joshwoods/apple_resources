

- HealthKit
-  HKMetadataKeyInsulinDeliveryReason 

Global Variable

# HKMetadataKeyInsulinDeliveryReason

The medical reason for administering insulin.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
let HKMetadataKeyInsulinDeliveryReason: String
```

## Discussion

This key is required for insulinDelivery samples. It takes an NSNumber object containing a HKInsulinDeliveryReason value.

## Topics

### Valid Delivery Reasons

Possible reasons for administering insulin.

enum HKInsulinDeliveryReason

Possible reasons for administering insulin.

