

- FSKit
- FSProbeResult
-  containerID 

Instance Property

# containerID

The container identifier, as found during the probe operation.

macOS 15.4+

``` source
var containerID: FSContainerIdentifier? { get }
```

## Discussion

This value is non-`nil` unless the result is FSMatchResult.notRecognized. For formats that lack a durable UUID on which to base a container identifier — which is only legal for a FSUnaryFileSystem — this value may be a random UUID.

## See Also

### Working with result properties

var name: String?

The resource name, as found during the probe operation.

var result: FSMatchResult

The match result, representing the recognition and usability of a probed resource.

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

