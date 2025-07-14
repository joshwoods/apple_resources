

- Technotes
-  TN3174: Diagnosing issues with the Apple Pay payment sheet on your website 

Article

# TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

## Overview

When the Apple Pay payment sheet is presented, a number of JavaScript events are triggered before the payment sheet is activated and ready for the customer to authenticate. Additionally, some events are triggered when the customer interacts with the payment sheet, such as changing their selected payment card with onpaymentmethodselected, or authorizing the transaction via user authentication with onpaymentauthorized.

The sequence of events depends on the configuration of the Apple Pay payment request. For example, including requiredShippingContactFields values may invoke the onshippingcontactselected event. For more information, see Getting started with Apple Pay on the Web.

For payments, the onvalidatemerchant, `onpaymentmethodselected`, and `onpaymentauthorized` event handlers are always invoked, so you must implement these methods and complete the events successfully with completeMerchantValidation, completePaymentMethodSelection and completePayment, respectively. However, most other events are optional and may be implemented as needed.

Some common payment sheet-related issues that you may encounter during your Apple Pay implementation include:

- “Apple Pay not available for this website” errors

- “Payment Failed” errors

- Payment sheet is unexpectedly dismissed

## Possible reasons for “Apple Pay not available for this website” errors

An “Apple Pay not available for this website” error can occur while presenting the payment sheet, most commonly for an invalid merchantIdentifier. To ensure your developer account is configured correctly, please go to Certificates, Identifiers &amp; Profiles and confirm the following:

- The `merchantIdentifier` provided to your payment session request matches an existing Merchant ID registered to your developer account.

- The `merchantIdentifier` also has an active payment processing certificate and merchant identity certificate.

- The domain provided to the payload of the `/startSession` or `/paymentSession` endpoints match the domain shown in your web browser’s address bar.

Note

The `/startSession` endpoint is being phased out and replaced by `/paymentSession`. See Requesting an Apple Pay Payment Session for more information.

## Possible reasons for “Payment Failed” errors

A “Payment Failed” error can occur while presenting the payment sheet, the most common reasons include:

- Invalid server configurations

- Invalid payment session request formatting

- Merchant validation issues

### Troubleshooting invalid server configurations

An invalid server configuration can cause several issues with your Apple Pay implementation, mostly due to the lack of security, trust and verification of your server’s authenticity via a mutual TLS connection. The most common issues with your server include:

- TLS handshake can’t be established.

- The server doesn’t support TLS 1.2 or later.

- The server uses unsupported TLS cipher suites.

- The server uses invalid or untrusted TLS certificates.

#### Issue: TLS handshake can’t be established

A TLS handshake can fail during the domain verification process. For example, your server may be misconfigured in the following ways:

- The server does not support TLS 1.2 or later.

- The server does not support one of the specified cipher suites for Apple Pay.

- The server is using invalid or untrusted TLS certificates.

#### Issue: Your server doesn’t support TLS 1.2 or later

Servers supporting Apple Pay on the Web need to use TLS 1.2 or later. Servers also need to be accessible by the Apple Pay merchant verification server and can’t be proxied or redirected. For additional guidance on using a strict allow list for Apple Pay IP addresses and merchant validation domains, see Setting up your Server.

#### Issue: Use of unsupported TLS cipher suites

Servers negotiating TLS connections for Apple Pay on the Web must use one of the supported cipher suites described in Setting up your Server. To debug which cipher suites are being negotiated between Apple’s domain verification client and your server, record a packet trace and review the cipher suites being offered by Apple’s domain verification server in the Client Hello packet. If a supported cipher suite is selected by your server, confirm this by reviewing the Server Hello packet sent back to the client. If there is an issue in the cipher suite negotiation then there will typically be a failure after the Client Hello packet.

#### Issue: Use of invalid or untrusted TLS certificates

Ensure you are using a valid TLS certificate. For example, make sure that this certificate is set up with a proper chain of trust and also adheres to Apple’s Certificate Transparency policy for Safari. You can double check this with a packet trace. Make sure the leaf certificate being used on your domain follows a valid chain of trust through the intermediate certificates to the root certificate. For additional guidance, see Requesting an Apple Pay Session.

### Troubleshooting payment session request formatting issues

The following topics provide guidance on resolving issues when requesting a payment session from Apple’s servers. When you experience an error, check the contents of the response body as it may contain a status message to determine where the issue occurred.

#### Issue: Unable to establish a secure connection or SSL handshake failure

This error typically indicates a merchant identity certificate issue. To resolve this error, please confirm the following:

- The payment session request:

  - Uses the `POST` method, not `GET`.

  - Values don’t contain accidental whitespace or spelling mistakes.

  - Uses the URL provided by the `validationURL` attribute.

- The `validationURL` attribute uses the `https://` scheme.

- The certificate is configured correctly.

- The correct certificate is used for the payment session, especially when managing multiple certificates.

- The correct private key is associated to the certificate.

- Your server is correctly configured. See Troubleshooting invalid server configurations.

To learn more about configuring a merchant identity certificate, see Configuring Your Environment. Additionally, see Setting Up Your Server to verify your server configuration is valid.

#### Issue: Received a payment session response error

**Error: 400 – Bad Request.** This error typically indicates a formatting issue. Review your request to ensure the request body isn’t empty and contains all required parameters.

**Error: 404 – Not Found.** When you begin the Apple Pay session, Apple responds with an `onvalidatemerchant` callback that includes a `validationURL`. This `validationURL` is the endpoint your server must use to validate itself and obtain a merchant session object. If you receive this error, make sure you are sending the payload to the exact URL provided in the `validationURL` field. Use a strict allow list for the merchant validation URLs. Send the payment session request from your server; never request the session from the client.

**Error: 417 – Expectation Failed.** The merchant ID is either not registered for Apple Pay service or not registered for the domain. If you receive this error, navigate to your Apple Developer account and confirm the following:

- You are passing the correct merchant ID, which is associated to the merchant identity certificate, within the request.

- There are both:

  - A fully configured payment processing certificate; and

  - A merchant identity certificate associated with the merchant ID.

- Your domain is registered and completed merchant domain verification successfully.

- The `initiativeContext` value is identical to the domain registered for your Apple Developer account.

Ensure the value provided in the `initiativeContext` request parameter is identical to the merchant ID registered for your Apple Developer account. If you have multiple merchant IDs, ensure the domain is registered to the same merchant ID associated with the merchant identity certificate used to secure the request.

The `initiativeContext` value should include subdomains, but shouldn’t contain the URL scheme (e.g. `https://`) or any paths. For example:

- **Valid:** `"secure.example.com"`

- **Invalid:** `"https://secure.example.com/request-session"`

If you plan to process payments on a root domain and subdomain—for example, `example.com` and `test.example.com`—register and verify each domain.

Note

Apple considers `www.` a subdomain, so if you plan to process payments for `example.com`, but customers can access your site at `www.example.com`, you may need to ensure you register and verify both domains.

**Error 500 – Internal Server Error.** This error indicates the request couldn’t be processed, or the request body is malformed or invalid. Please ensure your request body is a valid JSON.

### Troubleshooting merchant validation issues

The following topics provide guidance on resolving issues when debugging Apple Pay merchant validation. The most common merchant validation issues occur during your payment session, including:

- Mishandling of payment session merchant validation events.

- Requesting a payment session with invalid certificates or values.

- Failure to complete merchant validation on a payment session.

To learn more about validating sessions and your merchant payment requests, see Requesting an Apple Pay Payment Session for more information.

#### Issue: Mishandling of payment session merchant validation events

When the `onvalidatemerchant` event is triggered, your client-side code should ask your server to request an Apple Pay payment session from Apple over an mTLS connection.

The most common issues while handling merchant validation events occur when:

- You request an Apple Pay payment session from Apple.

- You invoke `completeMerchantValidation` after successfully receiving a payment session from Apple.

Please ensure your implementation is following the expected flows for these merchant validation events. For more information, see Providing Merchant Validation.

#### Issue: Requesting a payment session with invalid certificates or values.

You should create a new Apple Pay payment session for each transaction for your merchant. Your server posts a request using a mutual TLS (mTLS) connection by calling the Apple Pay server’s `/paymentSession` endpoint. Please confirm the following are true for your payment session request:

- The merchant identity certificate — a TLS certificate associated with your merchant ID — is used to authenticate your requests.

- The `merchantIdentifier` request parameter matches the same merchant ID value.

- For Apple Pay on the Web, use `"web"` for the `intiative` parameter. For the `initiativeContext` parameter, provide your fully qualified domain name associated with your Merchant Identity Certificate.

In resposne to the `POST` request, your server receives an opaque Apple Pay session object. The session expires after five (5) minutes. For Apple Pay on the WEb, you pass the session object to the completion method, `completeMerchantValidation`.

#### Issue: Failure to complete merchant validation

If you are able to successfully generate a payment session but encounter issues when you pass this session into `completeMerchantValidation`, this suggests one of a few potential issues:

- **The session data is not formatted as a JSON Object.** The `completeMerchantValidation` method does not support this data in string format; the data must be parsed as a JSON object before it can be successfully passed to the completion method.

- **The session data is incomplete or has been modified.** You should treat the payment session data you receive as *opaque* and should not modify or change any of its contents. The contents or format of this data can change periodically, so it’s better to mapping this data to a strongly-typed object while it is in transit through your server and passed to your client-side code.

- **The `initiativeContext` for the session does not match the browser domain or is not correctly formatted.** The value provided as the `initiativeContext` in the payment session request should exactly match the domain shown in the browser’s address bar. The `initiativeContext` value should include subdomains but should not contain the URL scheme (e.g. `https://`) or any paths.

- **You are mixing environments.** Ensure you are using the correct `merchantIdentifier` and `intiativeContext` for the environment you are requesting a payment session from (Sandbox or Production).

## Possible reasons why the payment sheet dismisses after initial presentation

When the Apple Pay payment sheet is presented but dismisses within a few seconds — for example, after the customer has clicked or tapped the Apple Pay button — typically one of the following issues has occurred:

- Merchant validation failed.

- At least one of the payment sheet event handler methods is implemented, but the equivalent completion method isn’t properly configured.

To determine if this payment sheet dismissal is due to a merchant validation failure, use Safari Web Inspector to log errors and objects when debugging merchant validation. Otherwise, please ensure the object passed to the event’s completion method is well-formed, contains valid data, and all required parameters.

For Apple Pay, each event handler has a thirty (30) second timeout. If the related completion method is not invoked within 30 seconds from the start of the event, the payment sheet will dismiss with an error. When the customer changes or updates fields on the payment sheet, their selections are shared through event handlers, allowing your website to respond to user input.

For example, for any of the customer-selected payment methods on the W3C `PaymentRequest` object — such as `shippingaddresschange` — when the browser calls one of these event handlers, you have 30 seconds to process the event and invoke the equivalent `updateWith` callback. Ensure any server requests to validate the shipping address occur within this 30-second period. For more information about using the W3C Payment Request API, see Setting up the payment request API to accept Apple Pay.

Important

For the `onpaymentauthorized` event, if your system takes longer than 30 seconds to process the payment, the customer may see the payment sheet dismiss with an error, even though you may eventually process the payment successfully.

If the payment sheet dismisses without user interaction, please confirm the following:

- Your event handler implementations invoke the equivalent completion method. Do not stub out any of these event handler or completion methods.

- Your event handler implementations don’t take longer than 30 seconds to execute. Check for any long-running operations in your client or server code that may prevent the completion methods from returning in a timely manner.

- Your event handler implementations aren’t triggering an exception, breakpoint, or error, preventing the equivalent completion methods invocation.

- The object provided to the completion handler is a well-formed and valid JSON object. Validate the structure outlined in the documentation for each event’s completion method. Additionally, ensure all required parameters are populated correctly.

Use Safari Web Inspector to identify which event handler completion method is related to an issue and then diagnose the underlying cause of the issue for that specific event, including both the event handler and completion method.

## Possible reasons why the payment sheet dismisses after customer authentication

You may experience situations where the payment sheet does not display a successful payment confirmation (the “Done” checkmark) after payment authentication, even though the transaction itself may have been successful. When this occurs, you have most likely failed to send a successful payment response back to Apple.

## Revision History

- **2024-06-25** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

