

- CryptoTokenKit
- TKSmartCard
-  transmit(\_:reply:) 

Instance Method

# transmit(\_:reply:)

Transmits data in Application Protocol Data Unit (APDU) format to the Smart Card.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func transmit(
    _ request: Data,
    reply: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func transmit(_ request: Data) async throws -> Data
```

## Parameters 

`request`  

The APDU request data.

`reply`  

response  
The APDU response data, or `nil` if communication with the Smart Card failed.

error  
Contains information about the the error preventing the transaction from being established.

The `NSError` object is created in the TKErrorDomain domain with a code in the TKError.Code enumeration.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func transmit(_ request: Data) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

You should only call this method after a session to the Smart Card has been established using the beginSession(reply:) method, and before the session is terminated using the endSession() method.

## See Also

### Communicating with the Smart Card

func beginSession(reply: (Bool, (any Error)?) -> Void)

Begins a session with the Smart Card.

func endSession()

Completes any pending transmissions and ends the session to the Smart Card.

