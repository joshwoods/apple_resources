

- FSKit
- FSProbeResult
-  notRecognized 

Type Property

# notRecognized

A probe result for an unrecognized file system.

macOS 15.4+

``` source
class var notRecognized: FSProbeResult { get }
```

## Discussion

An unrecognized probe result contains `nil` for its name and containerID properties.

## See Also

### Working with results

class func recognized(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system.

class func usable(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized and usable file system.

class func usableButLimited(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system that is usable, but with limited capabilities.

class var usableButLimited: FSProbeResult

A probe result for a recognized file system that is usable, but with limited capabilities.

