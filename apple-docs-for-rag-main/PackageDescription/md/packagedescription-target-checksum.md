

- PackageDescription
- Target
-  checksum 

Instance Property

# checksum

The checksum for the archive file that contains the referenced binary artifact.

SwiftPM 5.3+

``` source
final var checksum: String?
```

## Discussion

If you make a remote binary framework available as a Swift package, declare a remote, or *URL-based*, binary target in your package manifest with binaryTarget(name:url:checksum:). Always run `swift package compute-checksum path/to/MyFramework.zip` at the command line to make sure you create a correct SHA256 checksum.

For more information, see doc:distributing-binary-frameworks-as-swift-packages.

## See Also

### Creating a Binary Target

static func binaryTarget(name: String, path: String) -> Target

Creates a binary target that references an artifact on disk.

static func binaryTarget(name: String, url: String, checksum: String) -> Target

Creates a binary target that references a remote artifact.

var url: String?

The URL of a binary target.

