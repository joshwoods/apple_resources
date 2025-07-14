

- Uniform Type Identifiers
- UTType
-  symbolicLink 

Type Property

# symbolicLink

A type that represents a symbolic link.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var symbolicLink: UTType { get }
```

## Discussion

The identifier for this type is `public.symlink`.

This type conforms to UTTypeItem and UTTypeResolvable.

## See Also

### Apple file system objects

static var directory: UTType

A type that represents a file system directory, including packages and folders.

static var mountPoint: UTType

A type that represents a volume mount point.

static var aliasFile: UTType

A type that represents an alias file.

static var folder: UTType

A type that represents a user-browsable directory.

static var volume: UTType

A type that represents the root folder of a volume or mount point.

static var diskImage: UTType

A type that represents a data item that’s mountable as a volume.

