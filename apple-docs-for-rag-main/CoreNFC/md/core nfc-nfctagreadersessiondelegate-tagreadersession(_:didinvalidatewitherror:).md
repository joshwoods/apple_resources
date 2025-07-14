

- Core NFC
- NFCTagReaderSessionDelegate
-  tagReaderSession(\_:didInvalidateWithError:) 

Instance Method

# tagReaderSession(\_:didInvalidateWithError:)

Tells the delegate the reason for invalidating a reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
func tagReaderSession(
    _ session: NFCTagReaderSession,
    didInvalidateWithError error: any Error
)
```

**Required**

## Parameters 

`session`  

The session that has become invalid. Your app should discard any references it has to this session.

`error`  

The error indicating the reason for invalidation of the session.

