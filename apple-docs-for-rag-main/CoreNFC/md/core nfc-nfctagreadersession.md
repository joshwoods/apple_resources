

- Core NFC
-  NFCTagReaderSession 

Class

# NFCTagReaderSession

A reader session for detecting ISO7816, ISO15693, FeliCa, and MIFARE tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class NFCTagReaderSession
```

## Overview

Use NFCTagReaderSession to interact with one of the tag types listed in NFCTagType. To use this reader session, you must:

- Include the Near Field Communication Tag Reader Session Formats Entitlement in your app.

- Provide a non-empty string for the NFCReaderUsageDescription key in your app’s `info.plist` file.

To interact with ISO 7816 tags, add the list of the application identifiers supported in your app to the com.apple.developer.nfc.readersession.iso7816.select-identifiers information property list key. If you include the application identifier `D2760000850101`—the identifier for the NDEF application on MIFARE DESFire tags (NFC Forum T4T tag platform)—and the reader session finds a tag matching this identifier, it sends the delegate an NFCISO7816Tag tag object. To get the MIFARE DESFire tag as an NFCMiFareTag object, don’t include `D2760000850101` in the application identifier list.

Only one reader session of any type can be active in the system at a time. The system puts additional sessions in a queue and processes them in first-in, first-out (FIFO) order.

Important

Core NFC doesn’t support payment-related Application IDs.

## Topics

### Creating a Tag Reader Session

convenience init?(pollingOption: NFCTagReaderSession.PollingOption, delegate: any NFCTagReaderSessionDelegate, queue: DispatchQueue?)

Creates an NFC tag reader session.

struct PollingOption

Options that determine the type of tags that a reader session should detect during a polling sequence.

protocol NFCTagReaderSessionDelegate

A protocol that an object implements to receive callbacks sent from an NFC tag reader session.

### Connecting to a Tag

func connect(to: NFCTag, completionHandler: ((any Error)?) -> Void)

Connects the reader session to a tag and activates that tag.

var connectedTag: NFCTag?

The tag connected to the reader session.

### Restarting the Polling Sequence

func restartPolling()

Restarts the polling sequence so the reader session can discover new tags.

### Instance Methods

func connect(to: NFCTag) async throws

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

