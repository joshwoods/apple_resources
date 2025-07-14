

- Foundation
- URLResourceValues
-  mayHaveExtendedAttributes 

Instance Property

# mayHaveExtendedAttributes

A Boolean value that indicates the file may have extended attributes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var mayHaveExtendedAttributes: Bool? { get }
```

## Discussion

`true` if the file may have extended attributes; otherwise, `false` indicates there are none.

## See Also

### File values

var documentIdentifier: Int?

A value that the kernel assigns to identify a document.

var fileContentIdentifier: Int64?

A value APFS assigns that identifies a file’s content data stream.

var fileAllocatedSize: Int?

The total allocated size on-disk for the file, in bytes.

var fileProtection: URLFileProtection?

The protection level for the file.

var fileResourceIdentifier: (any NSCopying &amp; NSSecureCoding &amp; NSObjectProtocol)?

An identifier for comparing two file system objects for equality.

var fileResourceType: URLFileResourceType?

The type of the file system object.

var fileSecurity: NSFileSecurity?

The file system object’s security information.

var fileSize: Int?

The total file size, in bytes.

var isPurgeable: Bool?

A Boolean value that indicates whether the file system can delete a file when the system needs to free space.

var isSparse: Bool?

A Boolean value that indicates whether the file has sparse regions.

var isExecutable: Bool?

A Boolean value that indicates whether you can execute the file resource or search a directory resource.

var isRegularFile: Bool?

A Boolean value that indicates whether the resource is a regular file.

var mayShareFileContent: Bool?

A Boolean value that indicates whether the cloned files and their original files may share data blocks.

var totalFileAllocatedSize: Int?

The total allocated size of the file, in bytes.

var totalFileSize: Int?

The total displayable size of the file, in bytes.

