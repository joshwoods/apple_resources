

- Foundation
- URLResourceValues
-  documentIdentifier 

Instance Property

# documentIdentifier

A value that the kernel assigns to identify a document.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var documentIdentifier: Int? { get }
```

## Discussion

The kernel uses a document identifier, which can be either a file or a directory, to identify the document regardless of where it moves on a volume.

The document identifier survives safe-save operation, and is sticky to the path the kernel assigns. replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:) is the preferred safe-save API. The document identifier is persistent across system restarts, and doesn’t transfer when you copy the file. Document identifiers are only unique within a single volume. Not all volumes support this property.

## See Also

### File values

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

var totalFileAllocatedSize: Int?

The total allocated size of the file, in bytes.

var totalFileSize: Int?

The total displayable size of the file, in bytes.

