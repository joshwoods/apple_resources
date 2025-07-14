

- Uniform Type Identifiers
- UTType
-  volume 

Type Property

# volume

A type that represents the root folder of a volume or mount point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var volume: UTType { get }
```

## Discussion

The identifier for this type is `public.volume`.

This type conforms to UTTypeFolder.

## See Also

### Apple file system objects

static var directory: UTType

A type that represents a file system directory, including packages and folders.

static var symbolicLink: UTType

A type that represents a symbolic link.

static var mountPoint: UTType

A type that represents a volume mount point.

static var aliasFile: UTType

A type that represents an alias file.

static var folder: UTType

A type that represents a user-browsable directory.

static var diskImage: UTType

A type that represents a data item that’s mountable as a volume.

