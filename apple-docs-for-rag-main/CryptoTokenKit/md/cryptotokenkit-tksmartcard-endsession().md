

- CryptoTokenKit
- TKSmartCard
-  endSession() 

Instance Method

# endSession()

Completes any pending transmissions and ends the session to the Smart Card.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func endSession()
```

## Discussion

Calls to this method should balance calls to beginSession(reply:).

## See Also

### Communicating with the Smart Card

func beginSession(reply: (Bool, (any Error)?) -> Void)

Begins a session with the Smart Card.

func transmit(Data, reply: (Data?, (any Error)?) -> Void)

Transmits data in Application Protocol Data Unit (APDU) format to the Smart Card.

