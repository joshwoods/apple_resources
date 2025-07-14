

- Core NFC
-  NFCReaderSession 

Class

# NFCReaderSession

The abstract base class that represents a reader session for detecting NFC tags.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCReaderSession
```

## Overview

You do not create instances of this class. Instead, you create and use an instance of NFCNDEFReaderSession or NFCTagReaderSession. Only one reader session of any type can be active in the system at a time. The system puts additional sessions in a queue and processes them in FIFO order.

## Topics

### Determining Tag Reading Capability

class var readingAvailable: Bool

A Boolean value that determines whether the device supports NFC tag reading.

### Working with a Session

var delegate: AnyObject?

The delegate of the reader session.

var sessionQueue: dispatch_queue_t

The queue on which the reader session delegate callbacks and completion block handlers are dispatched.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NFCNDEFReaderSession
- NFCTagReaderSession
- NFCVASReaderSession

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

class NFCNDEFReaderSession

A reader session for detecting NFC Data Exchange Format (NDEF) tags.

class NFCTagReaderSession

A reader session for detecting ISO7816, ISO15693, FeliCa, and MIFARE tags.

class NFCVASReaderSession

A reader session for processing Value Added Service (VAS) tags.

protocol NFCReaderSessionProtocol

A general interface for interacting with a reader session.

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

