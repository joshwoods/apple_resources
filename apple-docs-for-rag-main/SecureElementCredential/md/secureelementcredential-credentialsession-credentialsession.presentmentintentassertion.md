

- SecureElementCredential
- CredentialSession
-  CredentialSession.PresentmentIntentAssertion 

Class

# CredentialSession.PresentmentIntentAssertion

An object that signals your app’s intention to make exclusive use of the device’s contactless features.

iOS 18.1+iPadOS 18.1+

``` source
final class PresentmentIntentAssertion
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

Create an instance of this type to obtain exclusive use of the user interface for a selected credential. This prevents interruptions to your app from Wallet, any other default contactless app, or other apps using the `SecureElementCredential` framework. The assertion expires when any of the following occur:

- The assertion instance deinitializes.

- You call the relinquish() method to indicate that you no longer need the assertion.

- The system’s 60-second timeout expires.

- The session encounters a CredentialSession.Event.cardEmulationTimeout, potentially caused by one of the `performTransaction` methods.

Apps can only acquire an assertion 15 seconds after relinquishing the previous assertion.

Any of the `transaction` methods automatically acquire an internal instance of the `PresentmentIntentAssertion`. Because of this, call `relinquish()` prior to using the transaction methods. The following sequence shows how this works in a SwiftUI application:

1.  Call acquirePresentmentAssertion() before showing any proprietary payment UI.

2.  Call relinquish() to stop using the assertion before invoking the transaction method.

3.  Invoke configuration() to start a `transactionTask`.

4.  Perform the transaction with the `transactionTask`.

5.  Call invalidate() after presenting the credential.

6.  Optionally, call acquirePresentmentAssertion() to finish up any proprietary payment UI.

7.  Call relinquish() again to end use of the assertion.

In a UIKit app, use the following approach:

1.  Call acquirePresentmentAssertion() prior to showing any proprietary payment UI.

2.  Call relinquish() to stop using the assertion before invoking the transaction API.

3.  Perform the transaction task.

4.  Optionally, call acquirePresentmentAssertion() to finish up any proprietary payment UI.

5.  Call relinquish() again to end use of the assertion.

## Topics

### Inspecting assertion state

var state: CredentialSession.PresentmentIntentAssertion.State

The state of a presentment intent assertion, indicating whether it’s currently valid.

enum State

An enumeration of possible states of a presentment intent assertion.

### Relinquishing presentment intent

func relinquish() async throws

End the presentment intent assertion.

## See Also

### Acquiring exclusive foreground privileges

func acquirePresentmentAssertion() async throws -> CredentialSession.PresentmentIntentAssertion

Indicates that the app intends to present a credential to a contactless interface.

