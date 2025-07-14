

- Core NFC
- NFCTagReaderSession
-  restartPolling() 

Instance Method

# restartPolling()

Restarts the polling sequence so the reader session can discover new tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func restartPolling()
```

## Discussion

After restarting the polling sequence, the reader session sends newly detected tags to the session’s delegate method tagReaderSession(_:didDetect:).

Note

Tags detected before polling restarts are invalid. Your app should discard any references it has to the invalid tags to free system resources.

Calling restartPolling() on an invalidated session has no effect. If you need to restart the reader session, create a new NFCTagReaderSession.

