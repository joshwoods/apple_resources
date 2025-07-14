

- Apple Pay on the Web
-  PaymentCredentialStatusResponse 

Structure

# PaymentCredentialStatusResponse

The response for information about the device’s support for Apple Pay and the payment credential status.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary PaymentCredentialStatusResponse {
 PaymentCredentialStatus paymentCredentialStatus;
};
```

## Overview

The response contains the paymentCredentialStatus of the device.

## Topics

### Payment credential status

paymentCredentialStatus

The status of the possible payment credentials that a person has provisioned in Wallet.

## See Also

### Apple Pay availability

Checking for Apple Pay availability

Use the Apple Pay JS API to check whether Apple Pay is available, to check whether a device has a payment credential provisioned in Wallet, and to determine when to display an Apple Pay button.

canMakePayments

Indicates whether the device supports Apple Pay.

applePayCapabilities

Indicates whether the device supports Apple Pay and whether the person has an active card in Wallet that qualifies for web payments.

canMakePaymentsWithActiveCard

Indicates whether the device supports Apple Pay and whether the user has an active card in Wallet.

Deprecated

PaymentCredentialStatus

Information about whether the device supports Apple Pay and the possible payment credentials the person has provisioned in Wallet.

