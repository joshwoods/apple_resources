

- Core NFC
- CardSession
- CardSession.Event
-  CardSession.Event.received(\_:) 

Case

# CardSession.Event.received(\_:)

The session received an Application Programming Data Unit (ADPU).

iOS 17.4+iPadOS 17.4+

``` source
case received(CardSession.APDU)
```

## Parameters 

`CardSession.APDU`  

The ADPU received from the session.

## See Also

### Events

case sessionStarted

The card session successfully started.

case readerDetected

The session detected the RF field of an external NFC reader.

class APDU

An Application Programming Data Unit (APDU) received from the NFC card reader.

case readerDeselected

The session lost the RF link or the currently-selected Application Identifier (AID) became deselected.

case sessionInvalidated(reason: CardSession.Error)

The session became invalid.

