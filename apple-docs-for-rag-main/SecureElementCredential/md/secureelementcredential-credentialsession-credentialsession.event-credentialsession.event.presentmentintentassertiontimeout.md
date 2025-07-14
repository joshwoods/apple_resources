

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.presentmentIntentAssertionTimeout 

Case

# CredentialSession.Event.presentmentIntentAssertionTimeout

The session’s presentment intent assertion timed out.

iOS 18.1+iPadOS 18.1+

``` source
case presentmentIntentAssertionTimeout
```

## Discussion

A CredentialSession.PresentmentIntentAssertion granted by a credential session lasts for 60 seconds. If it expires, your app needs to request a new one with acquirePresentmentAssertion().

## See Also

### Timeout events

case cardEmulationTimeout

The session’s card emulation timer expired.

