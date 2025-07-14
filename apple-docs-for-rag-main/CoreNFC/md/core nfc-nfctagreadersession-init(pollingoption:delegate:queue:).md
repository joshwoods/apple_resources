

- Core NFC
- NFCTagReaderSession
-  init(pollingOption:delegate:queue:) 

Initializer

# init(pollingOption:delegate:queue:)

Creates an NFC tag reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
convenience init?(
    pollingOption: NFCTagReaderSession.PollingOption,
    delegate: any NFCTagReaderSessionDelegate,
    queue: DispatchQueue? = nil
)
```

## Parameters 

`pollingOption`  

One or more options specifying the type of tags that the reader session scans for and detects.

`delegate`  

An object that handles callbacks from the reader session.

`queue`  

A dispatch queue that the reader session uses when making callbacks to the delegate. When queue is `nil`, the session creates and uses a serial dispatch queue.

## See Also

### Creating a Tag Reader Session

struct PollingOption

Options that determine the type of tags that a reader session should detect during a polling sequence.

protocol NFCTagReaderSessionDelegate

A protocol that an object implements to receive callbacks sent from an NFC tag reader session.

