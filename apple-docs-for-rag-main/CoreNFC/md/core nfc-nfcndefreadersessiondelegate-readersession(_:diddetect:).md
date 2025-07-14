

- Core NFC
- NFCNDEFReaderSessionDelegate
-  readerSession(\_:didDetect:) 

Instance Method

# readerSession(\_:didDetect:)

Tells the delegate that the session detected NFC tags with NDEF messages and enables read-write capability for the session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func readerSession(
    _ session: NFCNDEFReaderSession,
    didDetect tags: [any NFCNDEFTag]
)
```

## See Also

### Finding NDEF Messages and Tags

func readerSession(NFCNDEFReaderSession, didDetectNDEFs: [NFCNDEFMessage])

Tells the delegate that the session detected NFC tags with NDEF messages.

**Required**

