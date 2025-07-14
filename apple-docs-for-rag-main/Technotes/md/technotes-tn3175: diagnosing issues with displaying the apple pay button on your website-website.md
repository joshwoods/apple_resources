

- Technotes
-  TN3175: Diagnosing issues with displaying the Apple Pay button on your website 

Article

# TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

## Overview

There are two ways to display the Apple Pay button on your website— canMakePaymentsWithActiveCard and canMakePayments. Use `canMakePaymentsWithActiveCard` to display the Apple Pay button on any Apple Pay supported device with at least one provisioned card in Wallet. Otherwise, use `canMakePayments` to display the Apple Pay button on any Apple Pay supported device.

To test out different Apple Pay button configurations, see Apple Pay on the Web Interactive Demo. For more information about supporting Apple Pay on your website, see Apple Pay on the Web.

It is recommended that merchants display the Apple Pay button using JavaScript. This approach provides many benefits for developers, including:

- The button’s appearance uses an Apple-approved label, font, color, and style.

- The button’s contents retain ideal proportions as you change its size.

- The button’s label is automaticlly translated into the language setting of your device.

- The button’s corner radius can be configured to match the style of your UI.

- The button contains a system-provided alternative text label for VoiceOver support.

## Possible reasons for Apple Pay button display issues

Some common button display issues that you may encounter during your Apple Pay implementation include:

- The `canMakePaymentsWithActiveCard` method unexpectedly returns `false`.

- Apple Pay is displayed as a payment option although no cards are provisioned in Wallet.

- The Apple Pay button does nothing when tapped or clicked.

### Issue: The canMakePaymentsWithActiveCard method unexpectedly returns false

When you invoke the `canMakePaymentsWithActiveCard` method, it verifyies whether the device is capable of making Apple Pay payments, and the customer has at least one eligible card provisioned in Wallet. The method also verifies that the merchantIdentifier is registered for Apple Pay, has active certificates, and a verified merchant domain configured for your Apple Developer account.

If you are testing your Apple Pay integration with a device that has an active card in Wallet and still receive a `false` response from the `canMakePaymentsWithActiveCard`, there is an issue with your merchant ID configuration. Please confirm the following are correct:

- The `merchantIdentifier` passed to `canMakePaymentsWithActiveCard` is identical to the value registered for your Apple Developer account.

- The domain is registered and verified as a merchant domain for your Apple Developer account.

- The domain shown in your web browser’s address bar is identical to the merchant domain registered and verified for your Apple Developer account.

- Your devices are running iOS 10 and later, or macOS 10.12 and later. See Apple Pay on the web version history.

### Issue: Apple Pay is displayed as a payment option although no cards are provisioned in Wallet

This issue usually occurs when you have implemented the `canMakePayments` method (or no method at all), which returns `true` if the user has an Apple Pay capable device. If the customer selects the Apple Pay button in this state, you may prompt the customer to start an inline provisioning flow to add a card to their Wallet before proceeding with the payment flow. Once the card is added, the customer can automatically be brought back to your website to complete their purchase.

### Issue: The Apple Pay button does nothing when tapped or clicked

This issue often occurs when you provide invalid values to the properties of the  
ApplePayPaymentRequest after the customer taps or clicks the Apple Pay button. To resolve this issue, please confirm the following:

- The JavaScript Console shown from the Develop menu in Safari has no relevant errors.

- The payment request is configured with all of the required properties.

- The payment request properties all include a value; you cannot provide an empty or `nil` value.

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

