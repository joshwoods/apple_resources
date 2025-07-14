

- Core NFC
- NFCVASReaderSessionDelegate
-  readerSession(\_:didInvalidateWithError:) 

Instance Method

# readerSession(\_:didInvalidateWithError:)

Tells the delegate that the session become invalid and provides the reason.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readerSession(
    _ session: NFCVASReaderSession,
    didInvalidateWithError error: any Error
)
```

**Required**

## Parameters 

`session`  

The reader session that calls this method.

`error`  

The error indicating the reason for invalidating the session.

## Discussion

Your app should release any references it has to the reader session that called this method.

