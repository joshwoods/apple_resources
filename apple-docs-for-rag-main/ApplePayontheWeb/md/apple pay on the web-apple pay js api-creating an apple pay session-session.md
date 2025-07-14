

- Apple Pay on the Web
- Apple Pay JS API
-  Creating an Apple Pay Session 

Article

# Creating an Apple Pay Session

Provide a payment request and create the session.

## Overview

After you’ve checked that the Apple Pay JS API is available and is enabled on the current device, you’re ready to create the payment request and start the session. You can create a session only when a user explicitly asks to make a payment. For example, you can create the session when the user taps the Apple Pay button.

You supply two parameters to ApplePaySession:

- Version number. The Apple Pay version you’re using. (See Apple Pay on the web version history for version information.)

- Payment Request. An ApplePayPaymentRequest dictionary that contains all the information needed to display the payment sheet.

Creating an ApplePaySession object throws a JavaScript exception if any of the following occur:

- Any Apple Pay JS API is called from an insecure page.

- You pass an invalid payment request. Payment requests are invalid if they contain missing, unknown, or invalid properties, or if they have a total that is zero or less.

- You attempt to create the ApplePaySession outside of a user gesture handler. The exception error “Must create a new ApplePaySession from a user gesture handler” appears.

After the session is created, call its begin method to show the payment sheet.

Creating an Apple Pay Session shows creating a payment request and a new Apple Pay session, and displaying the payment sheet.

Listing 1. Example of constructing an Apple Pay session

```
var request = {
  countryCode: 'US',
  currencyCode: 'USD',
  supportedNetworks: ['visa', 'masterCard', 'amex', 'discover'],
  merchantCapabilities: ['supports3DS'],
  total: { label: 'Your Merchant Name', amount: '10.00' },
}
var session = new ApplePaySession(3, request);
```

## See Also

### Apple Pay session

Providing Merchant Validation

Validate your merchant identity and receive a session object for each payment request.

Requesting an Apple Pay payment session

Request a valid session from the Apple Pay server.

ApplePaySession

A session object for managing the payment process on the web.

