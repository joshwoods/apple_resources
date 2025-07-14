

- CryptoTokenKit
- TKSmartCard
-  withSession(\_:) 

Instance Method

# withSession(\_:)

Synchronously begins a session, executes the given closure, and ends the session.

iOSiPadOSMac CatalystmacOS 10.12+tvOSvisionOSwatchOS

``` source
func withSession(_ body: @escaping () throws -> T) throws -> T
```

## Parameters 

`body`  

A closure to be called in the context of the created session.

## See Also

### Transmitting Data

func send(ins: UInt8, p1: UInt8, p2: UInt8, data: Data?, le: Int?, reply: (Data?, UInt16, (any Error)?) -> Void)

Asynchronously transmits an APDU command to the card, returning the response in a completion handler.

func send(ins: UInt8, p1: UInt8, p2: UInt8, data: Data?, le: Int?) throws -> (sw: UInt16, response: Data)

Synchronously transmits an APDU command to the card and returns the response.

