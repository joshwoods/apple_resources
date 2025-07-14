

- PackageDescription
- Target
-  url 

Instance Property

# url

The URL of a binary target.

SwiftPM 5.3+

``` source
final var url: String?
```

## Discussion

The URL points to an archive file that contains the referenced binary artifact at its root.

Binary targets are only available on Apple platforms.

## See Also

### Creating a Binary Target

static func binaryTarget(name: String, path: String) -> Target

Creates a binary target that references an artifact on disk.

static func binaryTarget(name: String, url: String, checksum: String) -> Target

Creates a binary target that references a remote artifact.

var checksum: String?

The checksum for the archive file that contains the referenced binary artifact.

