

- Xcode
- Capabilities
-  Configuring Apple Pay support 

Article

# Configuring Apple Pay support

Process payments in your app using the payment information the user stores on their device.

## Overview

Apple Pay lets the user store payment information on their device and then use it to quickly purchase goods and services in your app. Your app creates a payment request that Apple Pay transfers between your app, the Apple Pay servers, and your payment provider. Apple Pay leverages the device’s Secure Element to help protect the user’s payment information.

To use Apple Pay in your app, add the capability to configure your app’s target with the necessary entitlements, and create a merchant identifier and payment processing certificate to help secure transaction data. For more detailed information about these steps, see the video Configuring Your Developer Account for Apple Pay.

Before you create a merchant identifier or select an existing one, follow the instructions in the Add a capability section of Adding capabilities to your app. When you reach the Capabilities library, choose Apple Pay. For watchOS apps with separate WatchKit extensions, add the capability to the WatchKit Extension’s target. The Apple Pay capability isn’t available for tvOS apps.

After you add the Apple Pay capability, Xcode updates your target’s entitlements file to include the Merchant IDs Entitlement, which is an array that contains the merchant identifiers you select. If you configure Xcode to automatically manage app signing, then at this point, Xcode also enables Apple Pay for your app’s App ID in your developer account.

Note

If you later remove the Apple Pay capability in Xcode, you must manually update your App ID’s configuration in your developer account to disable Apple Pay.

### Select or create a merchant identifier

A *merchant identifier* uniquely identifies you to Apple Pay as a merchant that’s able to accept payments. To allow your app to submit payment requests, specify at least one merchant identifier in your project’s configuration. After you add the Apple Pay capability, Xcode retrieves any existing merchant identifiers from your developer account and displays them in the capability’s Merchant IDs list. To fetch an updated list of your account’s merchant identifiers, click the refresh button below the list.

Enable one or more merchant identifiers in the list using their checkboxes. Conversely, uncheck a merchant identifier’s checkbox to disallow your app from using it. Xcode updates the Merchant IDs array — `com.apple.developer.in-app-payments` — in your target’s entitlements file to reflect any changes you make, and associates the selected merchant identifiers with the app’s App ID in your developer account.

Note

To avoid breaking a live version of your app that relies on the identifier association, Xcode doesn’t automatically dissociate a merchant identifier from your App ID when you deselect it in the capability.

To create a new merchant identifier, perform the following steps:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Apple Pay capability.

5.  Click the Add button (+) below the Merchant IDs list.

6.  Enter a merchant identifier in the dialog that appears. It’s preferrable to prefix a merchant identifier with `merchant.` and then append a custom string in reverse DNS notation.

7.  Click OK to save the new merchant identifier.

Xcode automatically registers the merchant identifier in your developer account, adds it to your target’s entitlements file, and selects it in the Merchant IDs list, indicating that your app is now able to use the new merchant identifier.

### Create a payment processing certificate

Before you can use your merchant identifier, you must generate a *payment processing certificate* — a digital certificate that secures transaction data and proves its origin. The Apple Pay servers use the certificate’s public key to encrypt payment data, and you or your payment service provider use the certificate’s private key to decrypt the data and process the payment. For more information on creating the certificate, see Create a payment processing certificate.

Note

If you use an e-commerce platform or payment service provider, please contact them for information about using their service with Apple Pay. For a list of supported platforms and providers, see Payment Platforms.

After you create your merchant identifier and payment processing certificate, use the PassKit framework to enable the collection of payments from within your app. For more information, see the Apple Pay documentation and the sample code Offering Apple Pay in Your App.

## See Also

### Commerce

Configuring Sign in with Apple support

Allow users to create an account and sign in to your app with their Apple Account.

Configuring Wallet support

Access the user’s Wallet to add, update, and display your app’s passes.

