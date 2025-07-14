

- Foundation
- URLResourceValues
-  canonicalPath 

Instance Property

# canonicalPath

The URL’s path as a canonical absolute file system path.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var canonicalPath: String? { get }
```

## See Also

### Universal resource values

var addedToDirectoryDate: Date?

The date the resource was created, or renamed into or within its parent directory.

var allValues: [URLResourceKey : Any]

A loosely-typed dictionary containing all keys and values.

var attributeModificationDate: Date?

The time the resource’s attributes were last modified.

var contentAccessDate: Date?

The date the resource was last accessed.

var contentModificationDate: Date?

The time the resource content was last modified.

var creationDate: Date?

The date the resource was created.

var customIcon: NSImage?

var effectiveIcon: AnyObject?

var generationIdentifier: (any NSCopying &amp; NSSecureCoding &amp; NSObjectProtocol)?

An opaque generation identifier which can be compared using `==` to determine if the data in a document has been modified.

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

