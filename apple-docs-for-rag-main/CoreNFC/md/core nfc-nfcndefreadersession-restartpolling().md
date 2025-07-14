

- Core NFC
- NFCNDEFReaderSession
-  restartPolling() 

Instance Method

# restartPolling()

Restarts the polling sequence so the reader session can discover new tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func restartPolling()
```

## Discussion

After restarting the polling sequence, the reader session sends newly detected tags to the session’s delegate method readerSession(_:didDetect:).

Note

Tags detected before polling restarts are invalid. Your app should discard any references it has to the invalid tags to free system resources.

Calling restartPolling() has no effect when:

- The session is invalid. If you need to restart the reader session, create a new NFCNDEFReaderSession.

- The session’s delegate doesn’t implement the readerSession(_:didDetect:) method. When this method is missing, the session calls readerSession(_:didDetectNDEFs:) to inform the delegate of new NDEF messages, then restarts the polling sequence.

