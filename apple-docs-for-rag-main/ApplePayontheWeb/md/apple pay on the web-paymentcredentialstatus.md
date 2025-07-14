

- Apple Pay on the Web
-  PaymentCredentialStatus 

Enumeration

# PaymentCredentialStatus

Information about whether the device supports Apple Pay and the possible payment credentials the person has provisioned in Wallet.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum PaymentCredentialStatus
```

## Overview

The following are possible return values:

`paymentCredentialsAvailable`  
Confirms that the device supports Apple Pay and there’s at least one active payment credential in Wallet that qualifies for payments on the web. Show an Apple Pay button and offer Apple Pay as the primary, but not necessarily sole, payment option.

`paymentCredentialStatusUnknown`  
Confirms that the device supports Apple Pay, but the Wallet information is unknown. Show an Apple Pay button and offer Apple Pay as a possible payment option.

`paymentCredentialsUnavailable`  
Confirms that the device supports Apple Pay and that the device doesn’t have any active payment credentials in Wallet. Offer Apple Pay as a payment option, but don’t make it the sole or default payment option. This gives people the option to set up Apple Pay as part of their purchase.

`applePayUnsupported`  
Indicates that the device doesn’t support Apple Pay. Don’t display an Apple Pay button or offer Apple Pay as a payment option.

## Topics

### Enumeration Cases

applePayUnsupported

paymentCredentialStatusUnknown

paymentCredentialsAvailable

paymentCredentialsUnavailable

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

PaymentCredentialStatusResponse

The response for information about the device’s support for Apple Pay and the payment credential status.

