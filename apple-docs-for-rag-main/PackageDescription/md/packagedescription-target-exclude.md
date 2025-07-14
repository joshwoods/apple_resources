

- PackageDescription
- Target
-  exclude 

Instance Property

# exclude

The paths to source and resource files that you don’t want to include in the target.

``` source
final var exclude: [String]
```

## Discussion

Excluded paths are relative to the target path. This property has precedence over the `sources` and `resources` properties.

## See Also

### Configuring File Locations

var path: String?

The path of the target, relative to the package root.

var sources: [String]?

The source files in this target.

var resources: [Resource]?

The explicit list of resource files in the target.

struct Resource

A resource to bundle with the Swift package.

var publicHeadersPath: String?

The path to the directory that contains public headers of a C-family target.

