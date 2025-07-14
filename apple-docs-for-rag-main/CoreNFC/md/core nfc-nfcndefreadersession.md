

- Core NFC
-  NFCNDEFReaderSession 

Class

# NFCNDEFReaderSession

A reader session for detecting NFC Data Exchange Format (NDEF) tags.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCNDEFReaderSession
```

## Overview

As with the NFCReaderSession base class, only one NFC NDEF reader session can be active in the system at a time. If you create an additional session, the system puts it in a queue and processes it in first-in, first-out (FIFO) order.

## Topics

### Creating a Session

init(delegate: any NFCNDEFReaderSessionDelegate, queue: dispatch_queue_t?, invalidateAfterFirstRead: Bool)

Creates and initializes a new NFC NDEF reader session.

protocol NFCNDEFReaderSessionDelegate

A protocol that an object implements to serve as an NDEF reader session delegate.

### Connecting to a Tag

func connect(to: any NFCNDEFTag, completionHandler: ((any Error)?) -> Void)

Connects the reader session to a tag and activates that tag.

### Restarting the Polling Sequence

func restartPolling()

Restarts the polling sequence so the reader session can discover new tags.

## Relationships

### Inherits From

- NFCReaderSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NFCReaderSessionProtocol
- NSObjectProtocol

## See Also

### Reader sessions

class NFCTagReaderSession

A reader session for detecting ISO7816, ISO15693, FeliCa, and MIFARE tags.

class NFCVASReaderSession

A reader session for processing Value Added Service (VAS) tags.

class NFCReaderSession

The abstract base class that represents a reader session for detecting NFC tags.

protocol NFCReaderSessionProtocol

A general interface for interacting with a reader session.

class NFCReaderSession

The abstract base class that represents a reader session for detecting NFC tags.

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

