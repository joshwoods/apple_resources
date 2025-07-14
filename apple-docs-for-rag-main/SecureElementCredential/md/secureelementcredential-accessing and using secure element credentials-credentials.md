

- SecureElementCredential
-  Accessing and using secure element credentials 

Article

# Accessing and using secure element credentials

Manage and use payment cards and other credentials.

## Overview

You can use the SecureElementCredential framework to store, manage, and use *credentials*, for example, contactless payment cards, transit passes, and corporate badges, that the system stores in the device’s Secure Element. The person using your app can then authenticate with features like Face ID and Touch ID to use their credentials.

`SecureElementCredential` provides UIKit and SwiftUI APIs to handle user authentication, and to temporarily give your app exclusive use of the device when presenting the credential. You can also receive notifications of credential-handling events. These include events like proximity to an NFC card reader, or the person performing a credential gesture like double tapping the side button of an iPhone.

You or your organization manage credentials and the embedded applet code you create for those credentials through the Apple Business Register (ABR). This framework allows your iOS app access to use those credentials.

### Create a credential session

The CredentialSession class is the central access point for working with credentials. To use it, first verify that the device is eligible to use credential sessions, by checking the value of isEligible. If eligible, create a session with startSession(). Then, fetch the available credentials with listCredentials(). If the credential you expect to use isn’t in the array returned by `listCredentials()`, call provisionCredential(configurationUUID:name:) to install the applet bundle that you submitted to ABR into the Secure Element, then list the credentials again.

The following example shows how to create a credential session in the context of a SwiftUI view that lists the available credentials. After the view instantiates and before it appears:

- The `.task` view modifier spawns a Task that calls a private `kickOff()` helper method.

- `kickOff()` makes the asynchronous calls to create the session and fetch an array of credentials from the Secure Element. This array can then populate a List.

```
```

When you first start the credential session, it’s in the default state, CredentialSession.State.management. In this state, you can perform the following actions:

- List credentials (as shown in the above example) with listCredentials().

- Provision new credentials with provisionCredential(configurationUUID:name:).

- Delete a credential with deleteCredential(_:)

Beyond the management state, there are two other credential session states:

- Wired state, for communicating directly with a credential stored in the Secure Element.

- Card emulation state, for using the credential with an NFC card reader.

### Obtain exclusive use of the user interface

Prior to presenting a credential for use with an NFC reader or performing transactions, your app can get exclusive use of the credential user interface. This exclusivity prevents interruptions from another app chosen as the default for contactless transactions, any other apps using the `SecureElementCredential` framework, and Wallet.

To gain exclusive use of the credential UI, obtain an instance of the CredentialSession.PresentmentIntentAssertion class. Hold on to this object until you finish using the credential. The following example shows an overview of this process:

```
```

The assertion expires when the object deinitializes, you call relinquish(), or after a 15-second timeout, whichever occurs first.

Note

You can acquire a maximum of two instances of CredentialSession.PresentmentIntentAssertion in one 80-second period.

### Enter wired mode

After obtaining a CredentialSession.Credential, many tasks require changing the state before you perform them. For example, you might need to maintain a credential by directly interacting with it in the Secure Element, which you can only do in the CredentialSession.State.wired(credential:) state. Credential maintenance tasks include exchanging keys and certificates with an installed credential.

Tip

Be aware that you can only perform these kinds of maintenance tasks if your app has owner-level access to the credential.

You can perform credential maintenance by transitioning the session state to CredentialSession.State.wired(credential:). Next, you send Application Protocol Data Unit (APDU) commands, as defined by ISO 7816-4, to the credential with the session’s transceive(_:) method. See the integration guide in the Apple Business Register for more information about the payloads for these calls.

Here’s how you enter wired mode and perform maintenance on a credential:

```
```

### Use wired mode in a UIKit app

You can also go into wired mode to get user authorization for using the credential, which authenticates with a passcode or biometric features like Face ID. This approach is useful for tasks like using the credential to perform web payments.

The following example shows how a UIKit-based app can get authorization and perform a transaction in wired mode. After getting the CredentialSession.PresentmentIntentAssertion as described above, it verifies that the selected credential is installed, and gets the first installed instance’s unique identifier. Using this unique identifier, it calls performWiredTransaction(using:over:instanceAID:) to present an authentication interface over the current UIScene. This call puts the session into wired mode, at which point the app can interact with the credential by calling transceive(_:).

For a web payment, an app might receive a token from a web service, and then ingest it by sending the token as the APDU payload of a `transceive(_:)` call. The credential then provides an APDU as the return value. It might take several exchanges to complete the transaction, after which the app exits wired mode by calling endWiredMode() and relinquishes the CredentialSession.PresentmentIntentAssertion.

```
```

The example above calls relinquish() before making the `performWiredTransaction(using:over:scene:)` call. This is because all methods that perform transactions acquire an internal instance of the presentment intent assertion on your behalf and automatically relinquish it. If you need to perform clean-up work after a transaction, acquire another assertion, subject to the limit of two assertions in an 80-second span.

### Use wired mode in a SwiftUI app

The flow is different when you use a SwiftUI View instead of a UIKit UIViewController, but the result is the same. The following example shows a SwiftUI view that presents the UI for performing a wired transaction. This example assumes you already acquired the CredentialSession.PresentmentIntentAssertion, and passed a CredentialSession and a CredentialSession.Credential to the view.

Before the view appears, the closure associated with the `View.task(priority:_:)` view modifier executes. This code fetches the current CredentialTransaction.Configuration and stores it in a state property. Next, the `View.transactionTask(_:action:)` closure runs. This closure gets the current credential, and from that, gets the unique identifier of the credential’s first instance. With instance ID, it can enter wired mode by calling performTransactionInWiredMode(using:instanceAID:) on the CredentialTransaction that the closure receives.

At this point, the SwiftUI sample is in the same state as the earlier UIKit example — you can make transceive(_:) calls to exchange APDUs with the installed credential to process the web transaction. When done, invalidate the configuration to exit wired mode and return to management mode.

```
```

### Perform card emulation

You can also use credentials for contactless transactions with NFC card readers. Implement the CredentialSessionWindowSceneDelegate protocol in your app to receive CredentialSessionWindowSceneEvent instances that describe NFC-related events. These events can occur when the device comes within range of an NFC card reader. Your app also gets an event when the person using the app performs a gesture to present an NFC display, like double-pressing the Home button or Side button.

To perform a contactless transaction, select an installed credential and then put the session into card emulation mode. In UIKit, you do this by calling performTransaction(using:over:options:). In the following example, the `performNFCTransaction()` method gets exclusive use of the contactless UI with acquirePresentmentAssertion(). Next, it verifies that the selected credential is installed and unwraps the current UIScene into a local variable. With these parameters, it calls `performTransaction(using:over:)` to begin the contactless transaction with the NFC reader.

The `performTransaction(using:over:)` method implicitly changes the session state to CredentialSession.State.cardEmulation(credential:). When the transaction completes, the example returns to management mode by calling endCardEmulation(), and relinquishes the contactless UI.

```
```

The SwiftUI equivalent uses the `transactionTask(_:action:)` view modifier to receive a CredentialTransaction from the view. Using this parameter, it calls performTransaction(using:options:) to enter card emulation mode.

```
```

### Performing wired actions and card emulation

The previous example assumes the credential is already installed and ready to use. It’s also possible to perform maintenance on a credential immediately before using it with an NFC reader. The following example shows how to do this. The `presentCredential()` method checks an internal `firstUse` flag to determine if it needs to perform up-front maintenance work. If so, it calls a private `personalizeCredentialInformation()` method to enter wired mode and perform the maintenance with one or more calls to transceive(_:).

After this method returns, the session has a current credential — the one it entered wired mode with — so it can enter card emulation mode with a call to performCardEmulationTransactionWithCurrentCredential(over:options:). On the other hand, if `presentCredential()` didn’t need to perform card maintenance, it calls performTransaction(using:over:options:) as before. In either case, the contactless transaction with the NFC reader proceeds, and the example calls endCardEmulation() when done.

```
```

In SwiftUI, the main difference is that the `transactionTask(_:action:)` view modifier provides a CredentialTransaction parameter when it executes your closure, so you call transaction-performing methods on this object.

In the following example, the code checks the `isFirstUse` flag in the closure passed to the `.transactionTask(_:action:)` view modifier and then performs any needed maintenance on the credential in wired mode. From there, the first-use case calls performCardEmulationTransactionWithCurrentCredential(options:) to enter card emulation mode with this credential. If the credential doesn’t require maintenance, which means the session is in management mode, the code calls performTransaction(using:options:), passing in the credential to use for the NFC transaction.

```
```

