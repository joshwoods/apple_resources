

- Apple Pay on the Web
- ApplePaySession
-  canMakePaymentsWithActiveCard Deprecated

Type Method

# canMakePaymentsWithActiveCard

Indicates whether the device supports Apple Pay and whether the user has an active card in Wallet.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
static Promise  canMakePaymentsWithActiveCard(
 DOMString merchantIdentifier
);
```

Deprecated

Use the applePayCapabilities method instead. The `canMakePaymentsWithActiveCard` method will continue to work on Safari browsers and always return `true` on third-party browsers.

## Parameters 

`merchantIdentifier`  

The merchant ID created when the merchant enrolled in Apple Pay.

## Return Value

`true` if the device supports Apple Pay and there is at least one active card in Wallet that is qualified for payments on the web; otherwise, `false`.

## Discussion

This method asynchronously contacts the Apple Pay servers as part of the verification process.

Per the Apple Pay on the Web Acceptable Use Guidelines, if you invoke the canMakePaymentsWithActiveCard API and determine that a user has an active card provisioned into Wallet, then Apple Pay must automatically be set as the default or sole payment option on any webpage where payments are accepted, such as the checkout page or product detail page. In all other situations, use canMakePayments instead.

Note that some cards, such as transit cards, are only enabled for POS payments and therefore won’t qualify for payments on the web.

The following code is an example of calling this method before displaying an Apple Pay button.

Determining whether to display an Apple Pay button

```
if (window.ApplePaySession) {
   var merchantIdentifier = 'example.com.store';
   var promise = ApplePaySession.canMakePaymentsWithActiveCard(merchantIdentifier);
   promise.then(function (canMakePayments) {
      if (canMakePayments)
         // Display Apple Pay Buttons here…
}); }
```

## See Also

### Apple Pay availability

Checking for Apple Pay availability

Use the Apple Pay JS API to check whether Apple Pay is available, to check whether a device has a payment credential provisioned in Wallet, and to determine when to display an Apple Pay button.

canMakePayments

Indicates whether the device supports Apple Pay.

applePayCapabilities

Indicates whether the device supports Apple Pay and whether the person has an active card in Wallet that qualifies for web payments.

PaymentCredentialStatus

Information about whether the device supports Apple Pay and the possible payment credentials the person has provisioned in Wallet.

PaymentCredentialStatusResponse

The response for information about the device’s support for Apple Pay and the payment credential status.

