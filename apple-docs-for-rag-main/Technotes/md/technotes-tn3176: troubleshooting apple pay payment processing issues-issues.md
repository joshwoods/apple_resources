

- Technotes
-  TN3176: Troubleshooting Apple Pay payment processing issues 

Article

# TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

## Overview

This technote covers debugging common Apple Pay payment processing issues. When an Apple Pay payment is requested by your app or website, Apple sends an encrypted payment token to you to verify its signature, decrypt its payment data, and validate the transaction. Often, these payment processing issues are caused by an invalid payment processing certificate, or by mishandling payment data by you or your payment service provider (PSP).

## Possible reasons for payment service provider errors while handling the Apple Pay payment token

Payment token validation that fail for your PSP are often due to an issue with your payment processing certificate or the format of your token. In either case, your PSP may be able to provide additional insight.

Please confirm the following with your PSP:

- The merchant ID value used throughout Apple Pay must be identical to the one you created in your Apple Developer account. If it is different, Apple will not be able to to decrypt the payment data.

- The merchant ID is associated with the correct payment processing certificate.

- The payment processing certificate is in an active state in your Apple Developer account.

- The merchantCapabilities array of the `ApplePayPaymentRequest`  
  contains only `supports3DS`.

- Your PSP is sending the authorization message in the format required by each payment network.

For more information about configuring your merchant identifier (ID) and certificates required for Apple Pay, see Configuring Your Environment.

## Possible reasons for payment token decryption errors

You validate a transaction by verifying the signature, decrypting the payment data, and verifying additional transaction details. A payment token’s payment data is encrypted using either elliptic curve cryptography (ECC) or RSA encryption. The encryption algorith used is based on the merchant capabilities of the initial payment request. The payment token can be decrypted by the merchant with the certificate private key or by the PSP on behalf of the merchant. For China mainland, decrypt via RSA; otherwise decrypt via ECC.

If you experience payment token-related decryption issues, please confirm the following:

- The PSP routes the payment to the correct payment network.

- The tokenization of the payment data doesn’t take too long or hasn’t timed out.

- The decrypted data is a valid JSON object.

- You receive a parseable JSON output when you attempt to decrypt a payment token, indicating a possible a key mismatch.

- No payment with the same `transactionId` shows as processed, indicating a transaction you’ve already credited.

- The merchant ID that you share with PSP is identical to the one you created in your Apple Developer account.

For more information, see Payment token format reference.

## Possible reasons for payment token processing errors

Once decrypted, the payment token is passed to the PSP for processing. If you experience payment token-related processing issues, please confirm the following:

- The cryptogram format is valid. For example, the `merchantCapabilities` property includes `supports3DS` (as well as `supportsEMV`, if you support China Union Pay transactions).

- Your PSP has assigned the correct Electronic Commerce Indicator (ECI) values for the transcation.

- Your certificate signing request (CSR) Apple uses to encrypt the payment token was generated for the correct environment (sandbox or production). and not mismatched.

- You aren’t reusing a previously processed payment token. Cryptograms are single-use and cannot be used over multiple transactions.

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

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

