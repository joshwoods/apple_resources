

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  requiredRecipientContactFields 

Instance Property

# requiredRecipientContactFields

An array that indicates which of the recipient’s contact details the merchant requires in order to process a disbursement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var requiredRecipientContactFields: [PKContactField] { get set }
```

## Discussion

The framework uses these details to display the input fields for name, email address, phone number, and so on on the payment sheet. The framework always shows them in a specific order, regardless of the order of API input.

## See Also

### Requesting recipient contact fields

var recipientContact: PKContact?

A contact object that describes the recipient.

