

- Core NFC
-  NFCISO15693RequestFlag 

Structure

# NFCISO15693RequestFlag

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
struct NFCISO15693RequestFlag
```

## Topics

### Initializers

init(rawValue: UInt8)

### Type Properties

static var RequestFlagAddress: NFCISO15693RequestFlag

A bit mask value that turns on the address flag.

Deprecated

static var RequestFlagDualSubCarriers: NFCISO15693RequestFlag

A bit mask value that turns on the subcarrier flag.

Deprecated

static var RequestFlagHighDataRate: NFCISO15693RequestFlag

A bit mask value that turns on the high data rate flag.

Deprecated

static var RequestFlagOption: NFCISO15693RequestFlag

A bit mask value that turns on the option flag.

Deprecated

static var RequestFlagProtocolExtension: NFCISO15693RequestFlag

A bit mask value that turns on the protocol extension flag.

Deprecated

static var RequestFlagSelect: NFCISO15693RequestFlag

A bit mask value that turns on the select flag.

Deprecated

static var address: NFCISO15693RequestFlag

static var commandSpecificBit8: NFCISO15693RequestFlag

static var dualSubCarriers: NFCISO15693RequestFlag

static var highDataRate: NFCISO15693RequestFlag

static var option: NFCISO15693RequestFlag

static var protocolExtension: NFCISO15693RequestFlag

static var select: NFCISO15693RequestFlag

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

### Enumerations

enum NFCFeliCaEncryptionId

enum NFCFeliCaPollingRequestCode

enum NFCFeliCaPollingTimeSlot

struct NFCISO15693ResponseFlag

enum ErrorCode

enum Mode

