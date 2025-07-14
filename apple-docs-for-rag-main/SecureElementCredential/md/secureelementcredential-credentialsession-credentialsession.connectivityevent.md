

- SecureElementCredential
- CredentialSession
-  CredentialSession.ConnectivityEvent 

Structure

# CredentialSession.ConnectivityEvent

An event that a credential receives during card emulation.

iOS 18.1+iPadOS 18.1+

``` source
struct ConnectivityEvent
```

## Topics

### Identifying the target instance

let instanceApplicationIdentifier: Data

The instance application identifier associated with the credential that receives an event.

### Inspecting event data

let data: Data

The data a credential receives during card emulation.

## Relationships

### Conforms To

- Sendable

## See Also

### Card emulation events

case connectivityEvent(CredentialSession.ConnectivityEvent)

A credential received a connectivity event during card emulation.

