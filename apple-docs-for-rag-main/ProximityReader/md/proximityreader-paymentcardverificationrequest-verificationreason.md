

- ProximityReader
- PaymentCardVerificationRequest
-  verificationReason 

Instance Property

# verificationReason

The reason you asked to verify someone’s card.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
let verificationReason: PaymentCardVerificationRequest.Reason
```

## Discussion

The system uses the supplied reason to display an appropriate message in the system UI about why they need to present their card.

## See Also

### Getting the request details

let currencyCode: String

The ISO 4217 code that indicates the currency type.

enum Reason

The reason for the verification request.

