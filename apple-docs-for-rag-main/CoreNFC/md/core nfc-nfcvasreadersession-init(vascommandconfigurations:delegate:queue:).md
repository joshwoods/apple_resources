

- Core NFC
- NFCVASReaderSession
-  init(vasCommandConfigurations:delegate:queue:) 

Initializer

# init(vasCommandConfigurations:delegate:queue:)

Creates a VAS reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(
    vasCommandConfigurations commandConfigurations: [NFCVASCommandConfiguration],
    delegate: any NFCVASReaderSessionDelegate,
    queue: dispatch_queue_t?
)
```

## Return Value

A newly initialized VAS reader session object.

## See Also

### Creating a VAS Reader Session

class NFCVASCommandConfiguration

An object providing the configuration for a GET VAS DATA command.

protocol NFCVASReaderSessionDelegate

A protocol that an object implements to receive callbacks from a VAS reader session.

