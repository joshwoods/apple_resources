

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Outputs
- PhotogrammetrySession.Outputs.Iterator
-  PhotogrammetrySession.Outputs.Iterator.Element 

Type Alias

# PhotogrammetrySession.Outputs.Iterator.Element

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias Element = PhotogrammetrySession.Outputs.Element
```

## See Also

### Output iteration

func next() async throws -> PhotogrammetrySession.Outputs.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

