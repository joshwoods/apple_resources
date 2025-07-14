

- Core NFC
- NFCFeliCaTag
-  requestSpecificationVersion(completionHandler:) 

Instance Method

# requestSpecificationVersion(completionHandler:)

Sends the Request Specification Version command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func requestSpecificationVersion(completionHandler: @escaping (Int, Int, Data, Data, (any Error)?) -> Void)
```

``` source
func requestSpecificationVersion() async throws -> (Int, Int, Data, Data)
```

**Required**

