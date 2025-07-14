

- Core NFC
- CardSession
- CardSession.Event
-  CardSession.Event.readerDetected 

Case

# CardSession.Event.readerDetected

The session detected the RF field of an external NFC reader.

iOS 17.4+iPadOS 17.4+

``` source
case readerDetected
```

## See Also

### Events

case sessionStarted

The card session successfully started.

case received(CardSession.APDU)

The session received an Application Programming Data Unit (ADPU).

class APDU

An Application Programming Data Unit (APDU) received from the NFC card reader.

case readerDeselected

The session lost the RF link or the currently-selected Application Identifier (AID) became deselected.

case sessionInvalidated(reason: CardSession.Error)

The session became invalid.

