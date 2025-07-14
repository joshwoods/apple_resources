

- Core NFC
- NFCNDEFReaderSession
-  init(delegate:queue:invalidateAfterFirstRead:) 

Initializer

# init(delegate:queue:invalidateAfterFirstRead:)

Creates and initializes a new NFC NDEF reader session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
init(
    delegate: any NFCNDEFReaderSessionDelegate,
    queue: dispatch_queue_t?,
    invalidateAfterFirstRead: Bool
)
```

## Parameters 

`delegate`  

The NFC NDEF delegate that handles reader session callbacks.

`queue`  

A queue onto which delegate callbacks are dispatched (the session retains the queue). When `queue` is `nil`, an internal serial dispatch queue is created for the session.

`invalidateAfterFirstRead`  

A Boolean value that indicates whether the session automatically invalidates after the first NDEF tag is successfully read.

## Discussion

When `invalidateAfterFirstRead` is false, the reader session can read multiple NFC tags. For each successful read, the delegate’s readerSession(_:didDetectNDEFs:) method delivers the message. A reader session that can read multiple tags terminates when the session times out or when the session is canceled by the client app (by calling invalidate()) or the user (via the user interface).

Note

When creating the reader session that your app uses to write an NDEF message to a tag, set `invalidateAfterFirstRead` to false. This keeps the session active so that your app can write a message to the tag.

When `invalidateAfterFirstRead` is true, the reader session automatically terminates after the first NFC tag is successfully read. In this scenario, the delegate receives the NFCReaderError.Code.readerSessionInvalidationErrorFirstNDEFTagRead status in readerSession(_:didInvalidateWithError:).

## See Also

### Creating a Session

protocol NFCNDEFReaderSessionDelegate

A protocol that an object implements to serve as an NDEF reader session delegate.

