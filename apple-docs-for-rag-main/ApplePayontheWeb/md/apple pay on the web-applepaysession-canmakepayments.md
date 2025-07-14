

- Apple Pay on the Web
- ApplePaySession
-  canMakePayments 

Type Method

# canMakePayments

Indicates whether the device supports Apple Pay.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
static boolean canMakePayments();
```

## Return Value

`true` if the device supports making payments with Apple Pay; otherwise, `false`.

## Mentioned in 

Checking for Apple Pay availability

## Discussion

This method only checks to ensure that the device supports processing payments with Apple Pay. It doesn’t verify whether or not the user has any provisioned cards in Wallet.

This method can be called any time.

## See Also

### Apple Pay availability

Checking for Apple Pay availability

Use the Apple Pay JS API to check whether Apple Pay is available, to check whether a device has a payment credential provisioned in Wallet, and to determine when to display an Apple Pay button.

applePayCapabilities

Indicates whether the device supports Apple Pay and whether the person has an active card in Wallet that qualifies for web payments.

canMakePaymentsWithActiveCard

Indicates whether the device supports Apple Pay and whether the user has an active card in Wallet.

Deprecated

PaymentCredentialStatus

Information about whether the device supports Apple Pay and the possible payment credentials the person has provisioned in Wallet.

PaymentCredentialStatusResponse

The response for information about the device’s support for Apple Pay and the payment credential status.

