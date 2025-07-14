

- RealityKit
- QueryResult
- QueryResult.Iterator
-  next() 

Instance Method

# next()

Advances to the next entity and returns it.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
mutating func next() -> Element?
```

## Return Value

Calling this method advances the iterator to the next entity and returns it. If there is no next element, returns `nil`.

