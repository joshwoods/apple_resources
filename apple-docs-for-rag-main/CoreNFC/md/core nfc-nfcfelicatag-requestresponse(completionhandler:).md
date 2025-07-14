

- Core NFC
- NFCFeliCaTag
-  requestResponse(completionHandler:) 

Instance Method

# requestResponse(completionHandler:)

Sends the Request Response command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func requestResponse(completionHandler: @escaping (Int, (any Error)?) -> Void)
```

``` source
func requestResponse() async throws -> Int
```

**Required**

