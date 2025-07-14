

- Core NFC
- NFCVASReaderSessionDelegate
-  readerSession(\_:didReceive:) 

Instance Method

# readerSession(\_:didReceive:)

Tells the delegate that the reader session received a VAS response.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readerSession(
    _ session: NFCVASReaderSession,
    didReceive responses: [NFCVASResponse]
)
```

**Required**

## Parameters 

`session`  

The reader session that calls this method.

`responses`  

An array of NFCVASResponse objects. The order of the response objects follows the sequence of `GET VAS DATA` sent to the tag by the reader session.

## Discussion

The reader session restarts polling when the detected tag moves from the session’s read range.

## See Also

### Receiving VAS Responses

class NFCVASResponse

An object representing the response from a single `GET VAS DATA` command.

