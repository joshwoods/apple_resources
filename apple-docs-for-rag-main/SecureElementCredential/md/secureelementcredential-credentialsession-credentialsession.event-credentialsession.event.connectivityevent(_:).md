

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.connectivityEvent(\_:) 

Case

# CredentialSession.Event.connectivityEvent(\_:)

A credential received a connectivity event during card emulation.

iOS 18.1+iPadOS 18.1+

``` source
case connectivityEvent(CredentialSession.ConnectivityEvent)
```

## Discussion

You might not receive this event if your app hasn’t acquired the CredentialSession.PresentmentIntentAssertion. If your app doesn’t have the presentment intent assertion, Wallet or another default app might respond to certain field events, depending on the device configuration.

## See Also

### Card emulation events

struct ConnectivityEvent

An event that a credential receives during card emulation.

