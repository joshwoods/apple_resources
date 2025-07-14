

- SecureElementCredential
- CredentialSession
- CredentialSession.PresentmentIntentAssertion
-  relinquish() 

Instance Method

# relinquish()

End the presentment intent assertion.

iOS 18.1+iPadOS 18.1+

``` source
final func relinquish() async throws
```

## Mentioned in 

Accessing and using secure element credentials

## Discussion

Call this function after your presentment task finishes.

A CredentialSession.PresentmentIntentAssertion times out after 60 seconds. If you don’t explicitly relinquish the object by then, the session produces CredentialSession.Event.presentmentIntentAssertionTimeout event, and invalidates this object.

