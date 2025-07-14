

- Core NFC
- NFCTagReaderSession
-  connectedTag 

Instance Property

# connectedTag

The tag connected to the reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
var connectedTag: NFCTag? { get }
```

## See Also

### Connecting to a Tag

func connect(to: NFCTag, completionHandler: ((any Error)?) -> Void)

Connects the reader session to a tag and activates that tag.

