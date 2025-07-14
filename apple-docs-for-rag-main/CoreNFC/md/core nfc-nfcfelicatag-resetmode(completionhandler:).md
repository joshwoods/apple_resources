

- Core NFC
- NFCFeliCaTag
-  resetMode(completionHandler:) 

Instance Method

# resetMode(completionHandler:)

Sends the Reset Mode command, as defined by the FeliCa card specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func resetMode(completionHandler: @escaping (Int, Int, (any Error)?) -> Void)
```

``` source
func resetMode() async throws -> (Int, Int)
```

**Required**

