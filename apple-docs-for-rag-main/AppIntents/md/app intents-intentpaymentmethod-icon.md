

- App Intents
- IntentPaymentMethod
-  icon 

Instance Property

# icon

The icon or image representing this payment method

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var icon: DisplayRepresentation.Image? { get }
```

## See Also

### Getting the payment details

var paymentType: IntentPaymentMethod.PaymentType

The kind of payment method, such as a credit card or bank account

var name: String?

The user-visible name of the payment method

var identificationHint: String?

A hint making it easier for the user to identify the payment method among others of similar name or type, such as the last several digits of a credit card number

enum PaymentType

Constants that describe the available payment options, such as credit cards or bank accounts.

