

- Apple Pay on the Web
- Apple Pay JS API
-  Providing Merchant Validation 

Article

# Providing Merchant Validation

Validate your merchant identity and receive a session object for each payment request.

## Overview

As soon as the system displays the payment sheet, the Apple Pay JS API calls your session object’s onvalidatemerchant event handler to verify that the request is coming from a valid merchant. It passes the function an ApplePayValidateMerchantEvent object that contains the validation URL.

Important

The URL you receive can vary, so always use the URL provided in the validationURL property. Your server must provide allow-listed access to all the validation URLs, specified in Setting Up Your Server.

In your onvalidatemerchant function:

1.  You call your server, passing it the URL from the event’s validationURL property.

2.  Your server uses the validation URL to request a session from the Apple Pay server, as described in Requesting an Apple Pay payment session. Never send the request for a merchant session from the client.

3.  In response, your server receives an opaque merchant session object.

4.  You pass the merchant session object to your Apple Pay session’s completeMerchantValidation method. You can use the merchant session object a single time. It expires five minutes after it is created.

## See Also

### Related Documentation

Configuring Your Environment

Create your Apple Pay merchant ID and certificates, and verify your domain.

Setting Up Your Server

Set up your server for secure communications with Apple Pay.

### Apple Pay session

Creating an Apple Pay Session

Provide a payment request and create the session.

Requesting an Apple Pay payment session

Request a valid session from the Apple Pay server.

ApplePaySession

A session object for managing the payment process on the web.

