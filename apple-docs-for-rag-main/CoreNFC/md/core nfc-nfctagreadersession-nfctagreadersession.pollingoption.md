

- Core NFC
- NFCTagReaderSession
-  NFCTagReaderSession.PollingOption 

Structure

# NFCTagReaderSession.PollingOption

Options that determine the type of tags that a reader session should detect during a polling sequence.

iOSiPadOSMac Catalyst

``` source
struct PollingOption
```

## Overview

You can combine options to have the reader session scan and detect different tag types at the same time.

## Topics

### Polling Options

static var iso14443: NFCTagReaderSession.PollingOption

The option for detecting ISO 7816-compatible and MIFARE tags.

static var iso15693: NFCTagReaderSession.PollingOption

The option for detecting ISO 15693 tags.

static var iso18092: NFCTagReaderSession.PollingOption

The option for detecting FeliCa tags.

### Initializers

init(rawValue: Int)

### Type Properties

static var pace: NFCTagReaderSession.PollingOption

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a Tag Reader Session

convenience init?(pollingOption: NFCTagReaderSession.PollingOption, delegate: any NFCTagReaderSessionDelegate, queue: DispatchQueue?)

Creates an NFC tag reader session.

protocol NFCTagReaderSessionDelegate

A protocol that an object implements to receive callbacks sent from an NFC tag reader session.

