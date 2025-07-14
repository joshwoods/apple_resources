

- Core NFC
- NFCNDEFReaderSessionDelegate
-  readerSessionDidBecomeActive(\_:) 

Instance Method

# readerSessionDidBecomeActive(\_:)

Tells the delegate that the reader session is active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func readerSessionDidBecomeActive(_ session: NFCNDEFReaderSession)
```

## Parameters 

`session`  

The active reader session. Only one session can be active at a time.

## Discussion

The reader session calls this method after the device begins scanning for new tags.

