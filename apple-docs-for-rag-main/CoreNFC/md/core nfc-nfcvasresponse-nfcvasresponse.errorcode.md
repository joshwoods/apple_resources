

- Core NFC
- NFCVASResponse
-  NFCVASResponse.ErrorCode 

Enumeration

# NFCVASResponse.ErrorCode

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum ErrorCode
```

## Topics

### Enumeration Cases

case dataNotActivated

case dataNotFound

case incorrectData

case success

case unsupportedApplicationVersion

case userIntervention

case wrongLCField

case wrongParameters

### Initializers

init?(rawValue: Int)

### Type Properties

static var VASErrorCodeDataNotActivated: NFCVASResponse.ErrorCode

A constant indicating that the data isn’t activated.

Deprecated

static var VASErrorCodeDataNotFound: NFCVASResponse.ErrorCode

A constant indicating that data wasn’t found.

Deprecated

static var VASErrorCodeIncorrectData: NFCVASResponse.ErrorCode

A constant indicating that the data is incorrect.

Deprecated

static var VASErrorCodeSuccess: NFCVASResponse.ErrorCode

A constant indicating that the `GET VAS DATA` command was successful.

Deprecated

static var VASErrorCodeUnsupportedApplicationVersion: NFCVASResponse.ErrorCode

A constant indicating an unsupported application version.

Deprecated

static var VASErrorCodeUserIntervention: NFCVASResponse.ErrorCode

A constant indicating that the tag requires user intervention.

Deprecated

static var VASErrorCodeWrongLCField: NFCVASResponse.ErrorCode

A constant indicating that the value in the Length Count field is wrong.

Deprecated

static var VASErrorCodeWrongParameters: NFCVASResponse.ErrorCode

A constant indicating that VAS command parameters are wrong.

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

enum NFCFeliCaPollingRequestCode

enum NFCFeliCaPollingTimeSlot

struct NFCISO15693RequestFlag

struct NFCISO15693ResponseFlag

enum Mode

