

- Core NFC
- NFCNDEFReaderSessionDelegate
-  readerSession(\_:didDetectNDEFs:) 

Instance Method

# readerSession(\_:didDetectNDEFs:)

Tells the delegate that the session detected NFC tags with NDEF messages.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func readerSession(
    _ session: NFCNDEFReaderSession,
    didDetectNDEFs messages: [NFCNDEFMessage]
)
```

**Required**

## Parameters 

`session`  

The reader session calling this method.

`messages`  

An array of the NDEF messages in the order they were discovered on the tag.

## Discussion

The reader session calls this method when it detects NFC tags with NDEF messages in the polling sequence. The session restarts polling when the detected tags are no longer within reading range of the iOS device.

Important

The reader session doesn’t call this method when the delegate provides the readerSession(_:didDetect:) method.

## See Also

### Finding NDEF Messages and Tags

func readerSession(NFCNDEFReaderSession, didDetect: [any NFCNDEFTag])

Tells the delegate that the session detected NFC tags with NDEF messages and enables read-write capability for the session.

