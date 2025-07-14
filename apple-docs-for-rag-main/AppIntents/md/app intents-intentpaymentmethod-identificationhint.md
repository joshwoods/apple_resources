

- App Intents
- IntentPaymentMethod
-  identificationHint 

Instance Property

# identificationHint

A hint making it easier for the user to identify the payment method among others of similar name or type, such as the last several digits of a credit card number

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var identificationHint: String? { get }
```

## See Also

### Getting the payment details

var paymentType: IntentPaymentMethod.PaymentType

The kind of payment method, such as a credit card or bank account

var name: String?

The user-visible name of the payment method

var icon: DisplayRepresentation.Image?

The icon or image representing this payment method

enum PaymentType

Constants that describe the available payment options, such as credit cards or bank accounts.

