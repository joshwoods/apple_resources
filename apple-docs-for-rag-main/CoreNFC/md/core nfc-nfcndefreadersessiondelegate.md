

- Core NFC
-  NFCNDEFReaderSessionDelegate 

Protocol

# NFCNDEFReaderSessionDelegate

A protocol that an object implements to serve as an NDEF reader session delegate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol NFCNDEFReaderSessionDelegate : NSObjectProtocol
```

## Topics

### Handling Session Activation

func readerSessionDidBecomeActive(NFCNDEFReaderSession)

Tells the delegate that the reader session is active.

### Finding NDEF Messages and Tags

func readerSession(NFCNDEFReaderSession, didDetectNDEFs: [NFCNDEFMessage])

Tells the delegate that the session detected NFC tags with NDEF messages.

**Required**

func readerSession(NFCNDEFReaderSession, didDetect: [any NFCNDEFTag])

Tells the delegate that the session detected NFC tags with NDEF messages and enables read-write capability for the session.

### Handling an Invalidated Session

func readerSession(NFCNDEFReaderSession, didInvalidateWithError: any Error)

Tells the delegate the reason for invalidating a reader session.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a Session

init(delegate: any NFCNDEFReaderSessionDelegate, queue: dispatch_queue_t?, invalidateAfterFirstRead: Bool)

Creates and initializes a new NFC NDEF reader session.

