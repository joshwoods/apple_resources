

- FSKit
- FSProbeResult
-  recognized(name:containerID:) 

Type Method

# recognized(name:containerID:)

Creates a probe result for a recognized file system.

macOS 15.4+

``` source
class func recognized(
    name: String,
    containerID: FSContainerIdentifier
) -> Self
```

## Parameters 

`name`  

The resource name, as found during the probe operation. If the file system doesn’t support names, or is awaiting naming, use an empty string.

`containerID`  

The container identifier, as found during the probe operation. If the file system doesn’t support durable identifiers, use a random UUID.

## See Also

### Working with results

class func usable(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized and usable file system.

class func usableButLimited(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system that is usable, but with limited capabilities.

class var usableButLimited: FSProbeResult

A probe result for a recognized file system that is usable, but with limited capabilities.

class var notRecognized: FSProbeResult

A probe result for an unrecognized file system.

