

- Core NFC
- CardSession
- CardSession.APDU
-  respond(response:) 

Instance Method

# respond(response:)

Respond to the session after receiving and processing an APDU.

iOS 17.4+iPadOS 17.4+

``` source
final func respond(response: Data) async throws
```

## Parameters 

`response`  

The APDU data to send as a response.

## Discussion

Your client must respond to each APDU it receives. Failing to respond throws an error. If your client disposes an APDU object without responding, the card emulation ends.

Warning

Only respond to a given APDU once. Calling this method more than once raises fatalError(_:file:line:). The exception to this is if the call throws CardSession.Error.transmissionError. In this case, you can retry the response by calling respond(response:) again.

