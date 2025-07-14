

- Core Data
- NSAsynchronousFetchRequest
-  init(fetchRequest:completionBlock:) 

Initializer

# init(fetchRequest:completionBlock:)

Initializes a new asynchronous fetch request configured with the provided fetch request and completion block.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    fetchRequest request: NSFetchRequest,
    completionBlock blk: ((NSAsynchronousFetchResult) -> Void)? = nil
)
```

