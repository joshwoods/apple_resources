

- Core NFC
-  NFCFeliCaPollingRequestCode 

Enumeration

# NFCFeliCaPollingRequestCode

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum NFCFeliCaPollingRequestCode
```

## Topics

### Enumeration Cases

case communicationPerformance

case noRequest

case systemCode

### Initializers

init?(rawValue: Int)

### Type Properties

static var PollingRequestCodeCommunicationPerformance: NFCFeliCaPollingRequestCode

A code that indicates a communication performance request.

Deprecated

static var PollingRequestCodeNoRequest: NFCFeliCaPollingRequestCode

A code that indicates no request.

Deprecated

static var PollingRequestCodeSystemCode: NFCFeliCaPollingRequestCode

A code that indicates a system code request.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum NFCFeliCaEncryptionId

enum NFCFeliCaPollingTimeSlot

struct NFCISO15693RequestFlag

struct NFCISO15693ResponseFlag

enum ErrorCode

enum Mode

