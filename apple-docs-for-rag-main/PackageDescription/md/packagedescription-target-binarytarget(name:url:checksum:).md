

- PackageDescription
- Target
-  binaryTarget(name:url:checksum:) 

Type Method

# binaryTarget(name:url:checksum:)

Creates a binary target that references a remote artifact.

SwiftPM 5.3+

``` source
static func binaryTarget(
    name: String,
    url: String,
    checksum: String
) -> Target
```

## Parameters 

`name`  

The name of the target.

`url`  

The URL to the binary artifact. This URL must point to an archive file that contains a binary artifact in its root directory.

`checksum`  

The checksum of the archive file that contains the binary artifact.

## Discussion

Binary targets are only available on Apple platforms.

## See Also

### Creating a Binary Target

static func binaryTarget(name: String, path: String) -> Target

Creates a binary target that references an artifact on disk.

var url: String?

The URL of a binary target.

var checksum: String?

The checksum for the archive file that contains the referenced binary artifact.

