

- Core NFC
- NFCFeliCaTag
-  writeWithoutEncryption(serviceCodeList:blockList:blockData:completionHandler:) 

Instance Method

# writeWithoutEncryption(serviceCodeList:blockList:blockData:completionHandler:)

Sends the Write Without Encryption command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data],
    blockData: [Data],
    completionHandler: @escaping (Int, Int, (any Error)?) -> Void
)
```

``` source
func writeWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data],
    blockData: [Data]
) async throws -> (Int, Int)
```

**Required**

## See Also

### Reading and Writing Without Encryption

func readWithoutEncryption(serviceCodeList: [Data], blockList: [Data], completionHandler: (Int, Int, [Data], (any Error)?) -> Void)

Sends the Read Without Encryption command, as defined by the FeliCa card specification, to the tag.

**Required**

