

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
- VideoReader.AsyncFrames.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
mutating func next() async throws -> TemporalFeature?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

