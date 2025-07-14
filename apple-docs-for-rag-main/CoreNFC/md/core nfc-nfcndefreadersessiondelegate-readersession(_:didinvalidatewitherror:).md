

- Core NFC
- NFCNDEFReaderSessionDelegate
-  readerSession(\_:didInvalidateWithError:) 

Instance Method

# readerSession(\_:didInvalidateWithError:)

Tells the delegate the reason for invalidating a reader session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func readerSession(
    _ session: NFCNDEFReaderSession,
    didInvalidateWithError error: any Error
)
```

**Required**

## Parameters 

`session`  

The session that has become invalid. Your app should discard any references it has to this session.

`error`  

The error indicating the reason for invalidation of the session.

