

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  recipientContact 

Instance Property

# recipientContact

A contact object that describes the recipient.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var recipientContact: PKContact? { get set }
```

## Discussion

If the merchant already has recipient contact information on file, set it here. Merchants should also include the corresponding contact fields in their requiredRecipientContactFields to ensure the data is visible on the payment sheet. Doing so enables people to select alternative contact information on the payment sheet, which merchants need to anticipate when they receive the final Apple Pay payment data.

## See Also

### Requesting recipient contact fields

var requiredRecipientContactFields: [PKContactField]

An array that indicates which of the recipient’s contact details the merchant requires in order to process a disbursement.

