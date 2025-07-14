

- ProximityReader
- PaymentCardReader
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether this device model supports Tap to Pay on iPhone.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
static let isSupported: Bool
```

## Mentioned in 

Adding support for Tap to Pay on iPhone to your app

## Discussion

For this property to be `true`, the device model must be iPhone XS or newer. This property doesn’t check the OS version.

