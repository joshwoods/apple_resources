

- Core NFC
-  NFCVASReaderSession 

Class

# NFCVASReaderSession

A reader session for processing Value Added Service (VAS) tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class NFCVASReaderSession
```

## Overview

Note

Using NFCVASReaderSession requires an entitlement from Apple. Updates will include information about the entitlement and a link to the entitlement request form.

## Topics

### Creating a VAS Reader Session

init(vasCommandConfigurations: [NFCVASCommandConfiguration], delegate: any NFCVASReaderSessionDelegate, queue: dispatch_queue_t?)

Creates a VAS reader session.

class NFCVASCommandConfiguration

An object providing the configuration for a GET VAS DATA command.

protocol NFCVASReaderSessionDelegate

A protocol that an object implements to receive callbacks from a VAS reader session.

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

class NFCNDEFReaderSession

A reader session for detecting NFC Data Exchange Format (NDEF) tags.

class NFCTagReaderSession

A reader session for detecting ISO7816, ISO15693, FeliCa, and MIFARE tags.

class NFCReaderSession

The abstract base class that represents a reader session for detecting NFC tags.

protocol NFCReaderSessionProtocol

A general interface for interacting with a reader session.

class NFCReaderSession

The abstract base class that represents a reader session for detecting NFC tags.

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

