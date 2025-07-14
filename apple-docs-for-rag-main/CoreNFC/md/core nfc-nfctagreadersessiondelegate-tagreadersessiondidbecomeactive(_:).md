

- Core NFC
- NFCTagReaderSessionDelegate
-  tagReaderSessionDidBecomeActive(\_:) 

Instance Method

# tagReaderSessionDidBecomeActive(\_:)

Tells the delegate that the reader session is active.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
func tagReaderSessionDidBecomeActive(_ session: NFCTagReaderSession)
```

**Required**

## Parameters 

`session`  

The active reader session. Only one session can be active at a time.

## Discussion

The reader session calls this method after the device begins scanning for new tags.

