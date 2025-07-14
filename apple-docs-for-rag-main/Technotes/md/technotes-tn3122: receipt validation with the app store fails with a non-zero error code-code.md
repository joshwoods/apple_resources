

- Technotes
-  TN3122: Receipt validation with the App Store fails with a non-zero error code 

Article

# TN3122: Receipt validation with the App Store fails with a non-zero error code

Identify common configurations that cause unsuccessful receipt validation with the App Store.

## Overview

Receipt validation with the App Store requires that you send a JSON object with the `receipt-data` and `password` keys, and optionally the `exclude-old-transactions` key as detailed in requestBody. The App Store responds with a value of `0` if validation was successful, and a status code if validation failed. This document lists reasons for unsuccessful validations.

## Encoding of the receipt data failed

Validating the receipt with the App Store requires encoding the receipt data using Base64 in your app before sending it to your server. Use Data.base64EncodedString(options:) as detailed in Fetch the Receipt Data or a Base64 algorithm of your choosing to encode the receipt data. if you use a different Base64 algorithm, confirm that it successfully covers and encodes all possible characters in a receipt.

## Shared secret is invalid

In App Store Connect, you can generate or regenerate a primary shared secret for all of your apps, or an app-specific shared secret for each of your apps. When you regenerate the primary shared secret, you invalidate the previous shared secret for all of your apps that use it. Confirm that the `password` key is set to the latest value of the primary shared secret for all of your apps that use it. See Generate a shared secret for details.

When you generate an app-specific shared secret for an app, that app can no longer use the primary shared secret. Confirm that `password` is set to the  
latest value of the app-specific shared secret for this app. The app-specific shared secret becomes invalid for the app when you regenerate it.

## Object posted to the App Store is invalid

On your server, create and format an object as JSON. This JSON object is a dictionary that contains the `receipt-data` and `password` keys. Each key pair in the dictionary is separated by a comma.

```
{
    "receipt-data": "your_Base64_encoded_receipt_data",
    "password": "your_shared_secret",
}
```

For receipts that contain auto-renewable subscriptions, optionally add `exclude-old-transactions` to the JSON object. The latest_receipt_info key contains the most recent entry for any subscriptions when `exclude-old-transactions` is set to `true` and all renewal entries, otherwise.

```
{
    "receipt-data": "your_Base64_encoded_receipt_data",
    "password": "your_shared_secret",
    "exclude-old-transactions": true
}
```

If `exclude-old-transactions` is absent in the JSON object, then the default value is `false`.

Important

On your server, be sure to send your JSON object as the payload of an HTTP POST request for receipt validation with the App Store.

## Validation request was posted to the incorrect URL

Use the sandbox URL to verify receipts when testing in the sandbox and while your app is in review:

```
https://sandbox.itunes.apple.com/verifyReceipt
```

Use the production URL to verify receipts when your app is live in the App Store:

```
https://buy.itunes.apple.com/verifyReceipt
```

First, verify your receipt with the production URL. If you receive a `21007` status code, as outlined in verifyReceipt, verify with the sandbox URL instead.

Note

TestFlight uses the sandbox environment for in-app purchases. See Testing at All Stages of Development with Xcode and Sandbox for details.

## Validate the receipt locally

Consider validating your receipt locally with the App Store to ensure your implementation works as designed. Use the `curl` command to test your JSON object.

To validate your receipt in the sandbox environment, run:

```
% curl -d 
'{
    "receipt-data": "your_Base64_encoded_receipt_data",
    "password": "your_shared_secret"
 }' 
 https://sandbox.itunes.apple.com/verifyReceipt
```

To validate your receipt in the production environment, run:

```
% curl -d 
'{
    "receipt-data": "your_Base64_encoded_receipt_data",
    "password": "your_shared_secret"
 }' 
 https://buy.itunes.apple.com/verifyReceipt
```

To validate your receipt in the production environment and limit the content of the `latest_receipt_info` key to only the most recent entry, run:

```
% curl -d 
'{
    "receipt-data": "your_Base64_encoded_receipt_data",
    "password": "your_shared_secret",
    "exclude-old-transactions": true
 }' 
 https://buy.itunes.apple.com/verifyReceipt
```

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-04-26** First published.

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

