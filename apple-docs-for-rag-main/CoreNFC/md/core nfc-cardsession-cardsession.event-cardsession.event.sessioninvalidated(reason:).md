

- Core NFC
- CardSession
- CardSession.Event
-  CardSession.Event.sessionInvalidated(reason:) 

Case

# CardSession.Event.sessionInvalidated(reason:)

The session became invalid.

iOS 17.4+iPadOS 17.4+

``` source
case sessionInvalidated(reason: CardSession.Error)
```

## Parameters 

`reason`  

The reason the session became invalid.

## Discussion

This is the last event produced by the event stream before the stream finishes. The reason can be any CardSession.Error except CardSession.Error.transmissionError.

## See Also

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

