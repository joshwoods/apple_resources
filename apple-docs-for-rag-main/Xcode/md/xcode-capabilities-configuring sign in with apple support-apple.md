

- Xcode
- Capabilities
-  Configuring Sign in with Apple support 

Article

# Configuring Sign in with Apple support

Allow users to create an account and sign in to your app with their Apple Account.

## Overview

Sign in with Apple gives your users the option to sign in to your app with their existing Apple Account instead of creating a separate username and password. All Apple devices support Sign in with Apple. For information about using this feature in the browser, see Sign in with Apple JS.

To use Sign in with Apple in your app, add the capability by configuring your app’s target in Xcode, set up the user interface and necessary authorizations, and register your domain with Apple’s relay service to ensure you can send emails to your users’ personal inboxes.

Note

If your app targets an OS version that predates the availability of Sign in with Apple, use the JavaScript library to provide the same functionality. For more information, see Incorporating Sign in with Apple into other platforms.

### Add the Sign in with Apple capability to your app

Follow the instructions in the Add a capability section of Adding capabilities to your app. When you reach the Capabilities library, choose Sign in with Apple. For watchOS apps with separate WatchKit extensions, add the capability to the WatchKit Extension’s target.

After you add the capability, Xcode updates the target’s entitlements to include the Sign in with Apple Entitlement — an array that contains a single string of `Default`, the value that represents normal operation. If you configure Xcode to automatically manage app signing, then at this point, Xcode also enables Sign in with Apple for your app’s App ID in your developer account.

Note

If you later remove the Sign in with Apple capability in Xcode, you must manually update your App ID’s configuration in your developer account to disable Sign in with Apple.

Users must provide their consent before Apple shares any information with your app. If you have a number of related apps — for example, an iOS app and a macOS app — group their App IDs so the user only needs to provide consent on the first device they use to access your app. For more information, see Group Apps for Sign in with Apple.

### Prompt the user to sign in with their Apple Account

After you add the Sign in with Apple capability to your Xcode project, update your app’s user interface to enable users to sign in with their Apple Account. For a reference implementation of the following steps, see the sample code Implementing User Authentication with Sign in with Apple.

- Add a Sign in with Apple button to your app’s user interface using ASAuthorizationAppleIDButton or WKInterfaceAuthorizationAppleIDButton.

- Add a handler for the button that creates an instance of ASAuthorizationAppleIDRequest. Make sure you set the request’s requestedScopes property. For more information, see ASAuthorization.Scope.

- Perform the authorization request with ASAuthorizationController, prompting the user to sign in with their Apple Account and consent to Apple sharing their details with your app.

- Implement the ASAuthorizationControllerDelegate protocol to determine the outcome of the authorization request and, if successful, receive the *credential* — an instance of ASAuthorizationAppleIDCredential that contains details about the user.

If your app stores account information on a remote server, send the credential’s contents to that server. The remote server verifies the data’s legitimacy with the Apple Account servers before creating or updating a user account. For more information, see Authenticating users with Sign in with Apple.

### Receive updates about Apple Account changes

If your app uses a remote server to manage user accounts, turn on server-to-server notifications so that the Apple Account servers notify you when users make changes to their Apple Account. The Apple Account servers send notifications when users change their mail forwarding preferences, delete their app account, or permanently delete their Apple Account. Use these notifications to maintain a canonical list of users. For more information, see Enabling Server to Server Notifications.

### Send emails to users’ hidden inboxes

If you include the email scope when you prompt the user for authorization, the system provides an option for that user to hide their real email address and instead use a unique, random forwarding email address that Apple provides. To help prevent spam and ensure that emails to users originate from your registered domains and email addresses, follow these steps:

- Register the domains and subdomains that you use for email communication.

- Register a list of unique email addresses that you use to send email.

- Authenticate your registered domains using the Sender Policy Framework (SPF) and DomainKeys Identified Mail (DKIM) protocol.

You must complete these steps before you can send emails to your users’ hidden inboxes. For more information, see Configure Private Email Relay Service.

## See Also

### Commerce

Configuring Apple Pay support

Process payments in your app using the payment information the user stores on their device.

Configuring Wallet support

Access the user’s Wallet to add, update, and display your app’s passes.

