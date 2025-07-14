

- PackageDescription
- Target
-  publicHeadersPath 

Instance Property

# publicHeadersPath

The path to the directory that contains public headers of a C-family target.

``` source
final var publicHeadersPath: String?
```

## Discussion

If this is `nil`, the directory is set to `include`.

## See Also

### Configuring File Locations

var path: String?

The path of the target, relative to the package root.

var exclude: [String]

The paths to source and resource files that you don’t want to include in the target.

var sources: [String]?

The source files in this target.

var resources: [Resource]?

The explicit list of resource files in the target.

struct Resource

A resource to bundle with the Swift package.

