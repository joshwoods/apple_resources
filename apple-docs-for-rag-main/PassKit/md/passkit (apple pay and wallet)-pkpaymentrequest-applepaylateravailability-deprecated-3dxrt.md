

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  applePayLaterAvailability Deprecated

Instance Property

# applePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOSwatchOS

``` source
var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability { get set }
```

Deprecated

Apple Pay Later is deprecated.

## Discussion

Defaults to enabled.

Use this property to suppress Apple Pay Later for a specific transaction. Only set this property if you have a specific requirement to disable Apple Pay Later.

Ensure you select the correct mode that matches your requirement, because the framework displays Apple Pay Later availability to the user.

Important

If you later decide to stop providing Apple Pay Later in your app, contact your acquirer or payment service provider (PSP) and notify them that you no longer wish to participate in the Mastercard Installments Program. You can always change this decision later.

## See Also

### Deprecated

enum ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

enum PKApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

