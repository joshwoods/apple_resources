

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Outputs
- PhotogrammetrySession.Outputs.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
mutating func next() async throws -> PhotogrammetrySession.Outputs.Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

## See Also

### Output iteration

typealias Element

