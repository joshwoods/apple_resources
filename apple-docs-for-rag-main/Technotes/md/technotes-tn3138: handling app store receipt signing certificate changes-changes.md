

- Technotes
-  TN3138: Handling App Store receipt signing certificate changes 

Article

# TN3138: Handling App Store receipt signing certificate changes

Ensure that your app’s local receipt validation is compatible with intermediate certificates that require using the SHA-256 algorithm.

## Overview

As part of ongoing efforts to improve security and privacy on Apple platforms, Apple is updating the App Store receipt signing intermediate certificate with one that uses the SHA-256 algorithm. This change affects the sandbox, TestFlight, and App Store environments, on the dates shown below:

| Date | Sandbox | TestFlight | App Store |
|----|----|----|----|
| January 24, 2025 | Uses SHA-256 certificate; SHA-1 certificate expires | Uses SHA-256 certificate; SHA-1 certificate expires | Uses SHA-256 certificate; SHA-1 certificate expires |
| August 16, 2023 |  | Uses SHA-256 certificate | Uses SHA-256 certificate |
| June 20, 2023 | Uses SHA-256 certificate |  |  |

The App Store receipt signing intermediate certificate is in the certificate chain that Apple uses to sign App Store receipts, which are the proof-of-purchase for apps and in-app purchases.

Important

If your app verifies App Store receipts on the device, follow the instructions outlined in this document to ensure that your receipt validation code is compatible with this change.

If your app performs on-device receipt validation, it needs to support SHA-256 algorithm to correctly verify Apple’s certificate chain. For more information, see Validating receipts on the device.

Starting January 24, 2025, apps that perform on-device receipt validation and don’t support a SHA-256 algorithm will fail their on-device receipt validation when the App Store updates the receipt. If your app prevents customers from accessing the app or premium content when receipt validation fails, your customers may lose access to their content.

Update your app to support certificates that use the SHA-256 algorithm if your app performs on-device receipt validation.

## Determine if your app is affected

Apps that are affected by Apple’s certificate update to SHA-256 include those that do the following:

- Perform on-device receipt validation, as described in Validating receipts on the device, and

- Use code to verify the chain of trust that doesn’t support the SHA-256 algorithm or relies on an expectation that the certificate encryption uses only SHA-1.

The certificate update does not affect any of the following transaction or receipt validation methods:

- Validating app and in-app purchase transactions using AppTransaction and Transaction.

- Server-to-server receipt verification using the verifyReceipt endpoint. For more information, see Validating receipts with the App Store.

Note

The verifyReceipt endpoint is deprecated. To validate receipts on your server, follow the steps in Validating receipts on the device on your server.

## Update your app to support SHA-256 certificates

Follow these guidelines to update your app to support certificates that use the SHA-256 algorithm for on-device receipt validation:

1.  If your app follows the instructions in Validating receipts on the device, the new certificate affects step 2, which involves verifying the certificate chain. Be sure your app uses the latest certificates from Apple PKI.

2.  Use cryptography code that supports SHA-256 algorithm. If you wrote your own code to verify receipts, update that code to use the SHA-256 algorithm. If your app uses a cryptography library, update the library to the latest version that supports SHA-256 algorithm.

3.  Test your app in the sandbox environment to ensure that your on-device receipt validation succeeds.

## Test your app receipt validation in the sandbox environment

Starting June 20, 2023, the sandbox environment produces app receipts that are signed using the SHA-256 intermediate certificate for apps running in iOS 16.6, tvOS 16.6, watchOS 9.6, and macOS 13.5. Follow these steps to test how your app handles the receipts:

1.  On a test device, sign in to the App Store with your Sandbox Apple ID.

2.  Launch the app.

3.  Perform one or more actions that cause the App Store to send an updated receipt to your app, such as the following:

    - Make an in-app purchase

    - Call SKReceiptRefreshRequest

    - Call restoreCompletedTransactions() or restoreCompletedTransactions(withApplicationUsername:).

4.  Verify that Apple signed the receipt with a SHA-256 certificate. Decode your app receipt as a PKCS \#7 container, then confirm that the `Receipt Creation Date` string, identified as ASN.1 Field Type 12, is set to June 20, 2023 or later in the sandbox environment. (In the production environment, that date is August 16, 2023 or later.)

5.  Ensure that your app calls its on-device receipt validation code with the new receipt.

6.  Check that your on-device receipt validation succeeds.

If your app successfully verifies the receipt and you’ve confirmed that the new receipt uses the updated certificate in its certificate chain, your app is ready for Apple’s SHA-256 intermediate certificate update.

Note

The receipt field SHA-1 Hash ASN.1 Field Type 5 is not affected by the certificate update. Use that field as described in step 5 of Validate the receipt.

## Revision History

- **2024-10-31** Added the SHA-1 expiry date. Noted that the `verifyReceipt` endpoint is now deprecated. Made other minor editorial changes.

- **2023-08-29** Updated date timeline.

- **2023-05-26** First published.

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

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

