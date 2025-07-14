

- CryptoTokenKit
- TKSmartCard
-  beginSession(reply:) 

Instance Method

# beginSession(reply:)

Begins a session with the Smart Card.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func beginSession(reply: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func beginSession() async throws -> Bool
```

## Parameters 

`reply`  

success  
Whether the session could be established successfully.

error  
Contains information about the error preventing the transaction from being established.

The `NSError` object is created in the TKErrorDomain domain with a code in the TKError.Code enumeration.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method will fail if there is already an existing session for the Smart Card.

Calls to this method must be balanced with calls to endSession().

## See Also

### Communicating with the Smart Card

func transmit(Data, reply: (Data?, (any Error)?) -> Void)

Transmits data in Application Protocol Data Unit (APDU) format to the Smart Card.

func endSession()

Completes any pending transmissions and ends the session to the Smart Card.

