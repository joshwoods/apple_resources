

- Core NFC
- NFCReaderSession
-  sessionQueue 

Instance Property

# sessionQueue

The queue on which the reader session delegate callbacks and completion block handlers are dispatched.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var sessionQueue: dispatch_queue_t { get }
```

## See Also

### Working with a Session

var delegate: AnyObject?

The delegate of the reader session.

