

- Core NFC
- NFCISO15693Tag
-  customCommand(requestFlags:customCommandCode:customRequestParameters:completionHandler:) 

Instance Method

# customCommand(requestFlags:customCommandCode:customRequestParameters:completionHandler:)

Sends a custom command (0xA0 to 0xDF command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func customCommand(
    requestFlags flags: NFCISO15693RequestFlag,
    customCommandCode: Int,
    customRequestParameters: Data,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

``` source
func customCommand(
    requestFlags flags: NFCISO15693RequestFlag,
    customCommandCode: Int,
    customRequestParameters: Data
) async throws -> Data
```

**Required**

## Discussion

This method inserts the icManufacturerCode after the command byte before appending the `customRequestParameters` when constructing the data packet that the method sends to the tag.

