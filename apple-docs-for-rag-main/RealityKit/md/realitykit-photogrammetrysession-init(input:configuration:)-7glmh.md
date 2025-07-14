

- RealityKit
- PhotogrammetrySession
-  init(input:configuration:) 

Initializer

# init(input:configuration:)

Creates a session from a sequence of samples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
convenience init(
    input: S,
    configuration: PhotogrammetrySession.Configuration = Configuration()
) throws where S : Sequence, S.Element == PhotogrammetrySample
```

## Parameters 

`input`  

The input `Sequence` that will be iterated once to yield all input data.

`configuration`  

The session-wide configuration to use for this session.

## Discussion

Creates a new session instance from a custom sequence of PhotogrammetrySample objects by iterating over the provided Sequence object.

The constructor will only use `makeIterator()` on `input` and will then iterate through the sequence only once. A provided iterator should be lazy, or a lazy Sequence and map used.

Note

To minimize memory usage, use lazy sequences that only create a PhotogrammetrySample as it iterates by making calls to `next()` on its associated IteratorProtocol.

## See Also

### Creating the session

convenience init(input: URL, configuration: PhotogrammetrySession.Configuration) throws

Creates a session from a specified directory of images.

static var isSupported: Bool

Returns `true` if the current hardware supports Object Capture.

