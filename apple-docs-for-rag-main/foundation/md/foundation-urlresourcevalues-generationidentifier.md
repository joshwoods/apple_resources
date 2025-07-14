

- Foundation
- URLResourceValues
-  generationIdentifier 

Instance Property

# generationIdentifier

An opaque generation identifier which can be compared using `==` to determine if the data in a document has been modified.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var generationIdentifier: (any NSCopying & NSSecureCoding & NSObjectProtocol)? { get }
```

## Discussion

For URLs which refer to the same file inode, the generation identifier will change when the data in the file’s data fork is changed (changes to extended attributes or other file system metadata do not change the generation identifier). For URLs which refer to the same directory inode, the generation identifier will change when direct children of that directory are added, removed or renamed (changes to the data of the direct children of that directory will not change the generation identifier). The generation identifier is persistent across system restarts. The generation identifier is tied to a specific document on a specific volume and is not transferred when the document is copied to another volume. This property is not supported by all volumes.

## See Also

### Universal resource values

var addedToDirectoryDate: Date?

The date the resource was created, or renamed into or within its parent directory.

var allValues: [URLResourceKey : Any]

A loosely-typed dictionary containing all keys and values.

var attributeModificationDate: Date?

The time the resource’s attributes were last modified.

var canonicalPath: String?

The URL’s path as a canonical absolute file system path.

var contentAccessDate: Date?

The date the resource was last accessed.

var contentModificationDate: Date?

The time the resource content was last modified.

var creationDate: Date?

The date the resource was created.

var customIcon: NSImage?

var effectiveIcon: AnyObject?

var hasHiddenExtension: Bool?

True for resources whose filename extension is removed from the localized name property.

var isAliasFile: Bool?

true if the resource is a Finder alias file or a symlink, false otherwise

var isExcludedFromBackup: Bool?

True if resource should be excluded from backups, false otherwise.

var isHidden: Bool?

True for resources normally not displayed to users.

var isPackage: Bool?

True for packaged directories.

var isReadable: Bool?

True if this process (as determined by EUID) can read the resource.

