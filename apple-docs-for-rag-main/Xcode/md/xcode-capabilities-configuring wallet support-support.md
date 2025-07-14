

- Xcode
- Capabilities
-  Configuring Wallet support 

Article

# Configuring Wallet support

Access the user’s Wallet to add, update, and display your app’s passes.

## Overview

The Wallet app on iOS and watchOS allows users to organize their *passes* — tickets, gift cards, loyalty cards, boarding passes, and the payment cards they use with Apple Pay. By integrating with PassKit (Apple Pay and Wallet), your app can access any related passes and allow the user to manage them.

To use Wallet in your app, add the capability by configuring your app’s target in Xcode and, optionally, specify which pass types your app supports. Follow the instructions in the Add a capability section of Adding capabilities to your app. When you reach the Capabilities library, choose Wallet. For watchOS apps with separate WatchKit extensions, add the capability to the WatchKit Extension’s target. The capability isn’t available for macOS or tvOS.

After you add the Wallet capability, Xcode updates your target’s entitlements file to include the Pass Type IDs Entitlement — an array containing the single wildcard value `$(TeamIdentifierPrefix)*`. This value allows your app to access passes of every pass type that you define in your developer account; use the configuration options of the capability to narrow the scope of accessible pass types to only those your app requires.

Important

The capability fetches and displays the pass type identifiers you register in your developer account; Xcode doesn’t provide a way to register them locally. For more information, see Create Wallet identifiers and certificates.

### Restrict your app to a subset of pass types

To minimize potential security risks and help protect the user’s privacy, follow these steps to provide your app with access to only the pass type identifiers it requires to function properly:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target from the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Wallet capability.

5.  Select the “Enable subset of pass types” option.

6.  Xcode enables all pass type identifiers by default; disable individual identifiers by unchecking their checkboxes.

Xcode updates the `com.apple.developer.pass-type-identifiers` array in the app’s entitlements file to include only the enabled pass type identifiers, and if present, removes the wildcard value.

After enabling the required pass type identifiers, use the passes() method of PKPassLibrary to retrieve the passes accessible to your app, or pass(withPassTypeIdentifier:serialNumber:) to fetch a specific pass. For more information on creating, distributing, and updating passes, see Wallet Passes.

## See Also

### Commerce

Configuring Apple Pay support

Process payments in your app using the payment information the user stores on their device.

Configuring Sign in with Apple support

Allow users to create an account and sign in to your app with their Apple Account.

