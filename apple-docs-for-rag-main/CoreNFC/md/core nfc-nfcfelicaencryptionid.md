

- Core NFC
-  NFCFeliCaEncryptionId 

Enumeration

# NFCFeliCaEncryptionId

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum NFCFeliCaEncryptionId
```

## Topics

### Enumeration Cases

case AES

case AES_DES

### Initializers

init?(rawValue: Int)

### Type Properties

static var aes: NFCFeliCaEncryptionId

An identifier that indicates the Advanced Encryption Standard (AES) encryption algorithm.

Deprecated

static var aes_des: NFCFeliCaEncryptionId

An identifier that indicates the Data Encryption Standard (DES) encryption algorithm.

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

enum NFCFeliCaPollingRequestCode

enum NFCFeliCaPollingTimeSlot

struct NFCISO15693RequestFlag

struct NFCISO15693ResponseFlag

enum ErrorCode

enum Mode

