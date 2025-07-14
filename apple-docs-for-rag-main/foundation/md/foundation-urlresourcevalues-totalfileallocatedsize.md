

- Foundation
- URLResourceValues
-  totalFileAllocatedSize 

Instance Property

# totalFileAllocatedSize

The total allocated size of the file, in bytes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var totalFileAllocatedSize: Int? { get }
```

## Discussion

The property returns `nil` if the information isn’t available. The allocated size in bytes may include space that metadata uses. This can be less than the value that totalFileSize returns after if it’s a compressed resource.

Note

This only applies to regular files.

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

var mayHaveExtendedAttributes: Bool?

A Boolean value that indicates the file may have extended attributes.

var isExecutable: Bool?

A Boolean value that indicates whether you can execute the file resource or search a directory resource.

var isRegularFile: Bool?

A Boolean value that indicates whether the resource is a regular file.

var mayShareFileContent: Bool?

A Boolean value that indicates whether the cloned files and their original files may share data blocks.

var totalFileSize: Int?

The total displayable size of the file, in bytes.

