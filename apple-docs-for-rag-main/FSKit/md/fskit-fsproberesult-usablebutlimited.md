

- FSKit
- FSProbeResult
-  usableButLimited 

Type Property

# usableButLimited

A probe result for a recognized file system that is usable, but with limited capabilities.

macOS 15.4+

``` source
class var usableButLimited: FSProbeResult { get }
```

## Discussion

This kind of probe result lacks the name, containerID, or both. Don’t return this result from probing a resource that isn’t limited.

## See Also

### Working with results

class func recognized(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system.

class func usable(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized and usable file system.

class func usableButLimited(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system that is usable, but with limited capabilities.

class var notRecognized: FSProbeResult

A probe result for an unrecognized file system.

