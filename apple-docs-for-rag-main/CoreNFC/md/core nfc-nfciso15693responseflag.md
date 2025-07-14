

- Core NFC
-  NFCISO15693ResponseFlag 

Structure

# NFCISO15693ResponseFlag

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct NFCISO15693ResponseFlag
```

## Topics

### Initializers

init(rawValue: UInt8)

### Type Properties

static var blockSecurityStatusBit5: NFCISO15693ResponseFlag

static var blockSecurityStatusBit6: NFCISO15693ResponseFlag

static var error: NFCISO15693ResponseFlag

static var finalResponse: NFCISO15693ResponseFlag

static var protocolExtension: NFCISO15693ResponseFlag

static var responseBufferValid: NFCISO15693ResponseFlag

static var waitTimeExtension: NFCISO15693ResponseFlag

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

struct NFCISO15693RequestFlag

enum ErrorCode

enum Mode

