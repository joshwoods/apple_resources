

- Core NFC
-  EncryptionId Deprecated

Type Alias

# EncryptionId

Encryption identifiers indicating the type of encryption algorithm used in the response of a Request Service V2 command.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
typealias EncryptionId = NFCFeliCaEncryptionId
```

## Topics

### Identifiers

static var aes: NFCFeliCaEncryptionId

An identifier that indicates the Advanced Encryption Standard (AES) encryption algorithm.

static var aes_des: NFCFeliCaEncryptionId

An identifier that indicates the Data Encryption Standard (DES) encryption algorithm.

## See Also

### Requesting Services

func requestService(nodeCodeList: [Data], completionHandler: ([Data], (any Error)?) -> Void)

Sends the Request Service command, as defined by the FeliCa card specification, to the tag.

**Required**

func requestServiceV2(nodeCodeList: [Data], completionHandler: (Int, Int, NFCFeliCaEncryptionId, [Data], [Data], (any Error)?) -> Void)

Sends the Request Service V2 command, as defined by the FeliCa card specification, to the tag.

**Required**

