

- SecureElementCredential
- CredentialSession
-  CredentialSession.Event 

Enumeration

# CredentialSession.Event

Events produced by a credential session, such as connectivity events and errors.

iOS 18.1+iPadOS 18.1+

``` source
enum Event
```

## Topics

### Credential events

case credentialFinishedInstalling(credential: CredentialSession.Credential)

The session finished installing a credential.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

### Card emulation events

case connectivityEvent(CredentialSession.ConnectivityEvent)

A credential received a connectivity event during card emulation.

struct ConnectivityEvent

An event that a credential receives during card emulation.

### NFC field events

case fieldStateChanged(info: CredentialSession.NFCFieldInformation)

The state of the NFC RF field changed during card emulation.

enum NFCFieldInformation

The state of an NFC RF field.

### Invalidation events

case sessionInvalidated(reason: CredentialSession.ErrorCode)

The session became invalidated.

enum ErrorCode

An error encountered by a credential session.

### Timeout events

case cardEmulationTimeout

The session’s card emulation timer expired.

case presentmentIntentAssertionTimeout

The session’s presentment intent assertion timed out.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling session events

var eventStream: AsyncStream&lt;CredentialSession.Event>

An asynchronous stream of session events.

