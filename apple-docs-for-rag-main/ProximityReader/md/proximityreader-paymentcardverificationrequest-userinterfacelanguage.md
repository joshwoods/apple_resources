

- ProximityReader
- PaymentCardVerificationRequest
-  userInterfaceLanguage 

Instance Property

# userInterfaceLanguage

The language to use when localizing the user interface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var userInterfaceLanguage: Locale.Language?
```

## Discussion

Setting this attribute only affects customer facing elements, screen elements, or audio targeted at the merchant (device owner) remains set to the language defined in the system settings. When you set this option to `nil`, the framework uses the person’s preferred language defined in System Settings.

