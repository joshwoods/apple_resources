

- PackageDescription
- Target
-  resources 

Instance Property

# resources

The explicit list of resource files in the target.

SwiftPM 5.3+

``` source
final var resources: [Resource]?
```

## See Also

### Configuring File Locations

var path: String?

The path of the target, relative to the package root.

var exclude: [String]

The paths to source and resource files that you don’t want to include in the target.

var sources: [String]?

The source files in this target.

struct Resource

A resource to bundle with the Swift package.

var publicHeadersPath: String?

The path to the directory that contains public headers of a C-family target.

