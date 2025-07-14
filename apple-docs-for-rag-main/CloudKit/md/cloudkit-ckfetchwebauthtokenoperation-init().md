

- CloudKit
- CKFetchWebAuthTokenOperation
-  init() 

Initializer

# init()

Creates an empty fetch operation.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+macOS 10.11+tvOS 9.1+visionOS 1.0+watchOS 3.0+

``` source
init()
```

## Discussion

You must set apiToken before you execute the operation or add it to a queue.

## See Also

### Creating a Fetch Token Operation

convenience init(apiToken: String)

Creates a fetch operation for the specified API token.

