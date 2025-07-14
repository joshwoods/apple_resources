

- SecureElementCredential
- CredentialSession
-  acquirePresentmentAssertion() 

Instance Method

# acquirePresentmentAssertion()

Indicates that the app intends to present a credential to a contactless interface.

iOS 18.1+iPadOS 18.1+

``` source
func acquirePresentmentAssertion() async throws -> CredentialSession.PresentmentIntentAssertion
```

## Return Value

A CredentialSession.PresentmentIntentAssertion object, representing exclusive access to presentment intent for a short time.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

Call this method when your app is in the foreground and showing a user interface appropriate for connecting to a contactless reader.

When you acquire this assertion, your app’s credential presentment can’t be interrupted by other entities’ presentment intents. Specifically, this prevents a default NFC app from interrupting when it detects an NFC reader’s RF field.

If another entity is already presenting a credential, calling this method throws an error. In this case, try calling the method again later.

Hold on to this instance as long as you need it (up to 60 seconds) to complete your credential presentment activity. When you’re done, call relinquish() to end the presentment assertion.

Repetitive acquisition of the assertion mechanism may result in a cooldown before being able to acquire the next assertion.

The exclusive use of the presentment intent expires after a predetermined timeout period. When this happens, the credential session’s event stream produces a CredentialSession.Event.presentmentIntentAssertionTimeout event.

## See Also

### Acquiring exclusive foreground privileges

class PresentmentIntentAssertion

An object that signals your app’s intention to make exclusive use of the device’s contactless features.

