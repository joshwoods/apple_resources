

- Core NFC
-  NFCTagReaderSessionDelegate 

Protocol

# NFCTagReaderSessionDelegate

A protocol that an object implements to receive callbacks sent from an NFC tag reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
protocol NFCTagReaderSessionDelegate : NSObjectProtocol
```

## Topics

### Handling Session Activation

func tagReaderSessionDidBecomeActive(NFCTagReaderSession)

Tells the delegate that the reader session is active.

**Required**

### Finding NFC Tags

func tagReaderSession(NFCTagReaderSession, didDetect: [NFCTag])

Tells the delegate that the session detected NFC tags.

**Required**

### Handling an Invalidated Session

func tagReaderSession(NFCTagReaderSession, didInvalidateWithError: any Error)

Tells the delegate the reason for invalidating a reader session.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a Tag Reader Session

convenience init?(pollingOption: NFCTagReaderSession.PollingOption, delegate: any NFCTagReaderSessionDelegate, queue: DispatchQueue?)

Creates an NFC tag reader session.

struct PollingOption

Options that determine the type of tags that a reader session should detect during a polling sequence.

