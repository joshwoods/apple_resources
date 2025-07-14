

- Core NFC
- NFCFeliCaTag
-  requestSystemCode(completionHandler:) 

Instance Method

# requestSystemCode(completionHandler:)

Sends the Request System Code command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func requestSystemCode(completionHandler: @escaping ([Data], (any Error)?) -> Void)
```

``` source
func requestSystemCode() async throws -> [Data]
```

**Required**

