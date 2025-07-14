

- Foundation
- NSFileVersion
-  getNonlocalVersionsOfItem(at:completionHandler:) 

Type Method

# getNonlocalVersionsOfItem(at:completionHandler:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func getNonlocalVersionsOfItem(
    at url: URL,
    completionHandler: @escaping ([NSFileVersion]?, (any Error)?) -> Void
)
```

``` source
class func nonlocalVersionsOfItem(at url: URL) async throws -> [NSFileVersion]
```

