

- Core NFC
-  NFCVASReaderSessionDelegate 

Protocol

# NFCVASReaderSessionDelegate

A protocol that an object implements to receive callbacks from a VAS reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
protocol NFCVASReaderSessionDelegate : NSObjectProtocol
```

## Topics

### Handling Session Activation

func readerSessionDidBecomeActive(NFCVASReaderSession)

Tells the delegate that the reader session is active.

### Receiving VAS Responses

func readerSession(NFCVASReaderSession, didReceive: [NFCVASResponse])

Tells the delegate that the reader session received a VAS response.

**Required**

class NFCVASResponse

An object representing the response from a single `GET VAS DATA` command.

### Handling an Invalidated Session

func readerSession(NFCVASReaderSession, didInvalidateWithError: any Error)

Tells the delegate that the session become invalid and provides the reason.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a VAS Reader Session

init(vasCommandConfigurations: [NFCVASCommandConfiguration], delegate: any NFCVASReaderSessionDelegate, queue: dispatch_queue_t?)

Creates a VAS reader session.

class NFCVASCommandConfiguration

An object providing the configuration for a GET VAS DATA command.

