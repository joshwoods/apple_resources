

- Core NFC
- CardSession
-  CardSession.Event 

Enumeration

# CardSession.Event

A type that enumerates events produced by a card session.

iOS 17.4+iPadOS 17.4+

``` source
enum Event
```

## Topics

### Events

case sessionStarted

The card session successfully started.

case readerDetected

The session detected the RF field of an external NFC reader.

case received(CardSession.APDU)

The session received an Application Programming Data Unit (ADPU).

class APDU

An Application Programming Data Unit (APDU) received from the NFC card reader.

case readerDeselected

The session lost the RF link or the currently-selected Application Identifier (AID) became deselected.

case sessionInvalidated(reason: CardSession.Error)

The session became invalid.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling card events

var eventStream: CardSession.EventStream

An asynchronous sequence of events from the card session.

class EventStream

An asynchronous sequence of events produced by a card session.

