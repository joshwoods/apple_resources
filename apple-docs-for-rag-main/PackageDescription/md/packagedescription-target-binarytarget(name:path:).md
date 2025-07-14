

- PackageDescription
- Target
-  binaryTarget(name:path:) 

Type Method

# binaryTarget(name:path:)

Creates a binary target that references an artifact on disk.

SwiftPM 5.3+

``` source
static func binaryTarget(
    name: String,
    path: String
) -> Target
```

## Parameters 

`name`  

The name of the target.

`path`  

The path to the binary artifact. This path can point directly to a binary artifact or to an archive file that contains the binary artifact at its root.

## Discussion

Binary targets are only available on Apple platforms.

## See Also

### Creating a Binary Target

static func binaryTarget(name: String, url: String, checksum: String) -> Target

Creates a binary target that references a remote artifact.

var url: String?

The URL of a binary target.

var checksum: String?

The checksum for the archive file that contains the referenced binary artifact.

