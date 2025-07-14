

- Core NFC
- NFCVASCommandConfiguration
-  NFCVASCommandConfiguration.Mode 

Enumeration

# NFCVASCommandConfiguration.Mode

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum Mode
```

## Topics

### Enumeration Cases

case normal

case urlOnly

### Initializers

init?(rawValue: Int)

### Type Properties

static var VASModeNormal: NFCVASCommandConfiguration.Mode

A constant that indicates the Full VAS Protocol mode.

Deprecated

static var VASModeURLOnly: NFCVASCommandConfiguration.ModeDeprecated

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

enum NFCFeliCaPollingRequestCode

enum NFCFeliCaPollingTimeSlot

struct NFCISO15693RequestFlag

struct NFCISO15693ResponseFlag

enum ErrorCode

