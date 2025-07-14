

- Core NFC
- NFCFeliCaTag
-  readWithoutEncryption(serviceCodeList:blockList:completionHandler:) 

Instance Method

# readWithoutEncryption(serviceCodeList:blockList:completionHandler:)

Sends the Read Without Encryption command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data],
    completionHandler: @escaping (Int, Int, [Data], (any Error)?) -> Void
)
```

``` source
func readWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data]
) async throws -> (Int, Int, [Data])
```

**Required**

## See Also

### Reading and Writing Without Encryption

func writeWithoutEncryption(serviceCodeList: [Data], blockList: [Data], blockData: [Data], completionHandler: (Int, Int, (any Error)?) -> Void)

Sends the Write Without Encryption command, as defined by the FeliCa card specification, to the tag.

**Required**

