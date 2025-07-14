

- Core NFC
- CardSession
-  CardSession.APDU 

Class

# CardSession.APDU

An Application Programming Data Unit (APDU) received from the NFC card reader.

iOS 17.4+iPadOS 17.4+

``` source
final class APDU
```

## Topics

### Receiving data

let payload: Data

The APDU data received from the NFC reader.

### Communicating with the card session

func respond(response: Data) async throws

Respond to the session after receiving and processing an APDU.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Events

case sessionStarted

The card session successfully started.

case readerDetected

The session detected the RF field of an external NFC reader.

case received(CardSession.APDU)

The session received an Application Programming Data Unit (ADPU).

case readerDeselected

The session lost the RF link or the currently-selected Application Identifier (AID) became deselected.

case sessionInvalidated(reason: CardSession.Error)

The session became invalid.

