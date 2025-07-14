

- Core NFC
- NFCFeliCaTag
-  requestService(nodeCodeList:completionHandler:) 

Instance Method

# requestService(nodeCodeList:completionHandler:)

Sends the Request Service command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func requestService(
    nodeCodeList: [Data],
    completionHandler: @escaping ([Data], (any Error)?) -> Void
)
```

``` source
func requestService(nodeCodeList: [Data]) async throws -> [Data]
```

**Required**

## See Also

### Requesting Services

func requestServiceV2(nodeCodeList: [Data], completionHandler: (Int, Int, NFCFeliCaEncryptionId, [Data], [Data], (any Error)?) -> Void)

Sends the Request Service V2 command, as defined by the FeliCa card specification, to the tag.

**Required**

typealias EncryptionId

Encryption identifiers indicating the type of encryption algorithm used in the response of a Request Service V2 command.

Deprecated

