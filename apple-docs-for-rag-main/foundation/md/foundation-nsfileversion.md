

- Foundation
-  NSFileVersion 

Class

# NSFileVersion

A snapshot of a file at a specific point in time.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSFileVersion
```

## Overview

Use the methods of this class to access, create, and manage file revisions in your app.

Each file version instance contains metadata about a single revision, including the location of the associated file, the modification date of the revision, and whether the revision is discardable.

In Mac apps, you can use file version objects to track changes to a local file over time and to prevent the loss of data during editing. When managing local versions, the document architecture creates versions at specific points in the lifetime of your application. Your application can also create versions explicitly at times that your application designates as appropriate.

In addition to managing local files, the system also uses this class to manage cloud-based files. For files in the cloud, there is usually only one version of the file at any given time. However, additional file versions may be created in cases where two different computers attempt to save the file to the cloud at the same time. In that case, one file is chosen as the current version and any other versions are tagged as being in conflict with the original. Conflict versions are reported to the appropriate file presenter objects and should be resolved as soon as possible so that the corresponding files can be removed from the cloud.

## Topics

### Getting the Version of a File

class func currentVersionOfItem(at: URL) -> NSFileVersion?

Returns the most recent version object for the file at the specified URL.

class func otherVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns all versions of the specified file except the current version.

class func version(itemAt: URL, forPersistentIdentifier: Any) -> NSFileVersion?

Returns the version of the file that has the specified persistent ID.

class func temporaryDirectoryURLForNewVersionOfItem(at: URL) -> URL

Creates and returns a temporary directory to use for saving the contents of the file.

### Creating a New Version

class func addOfItem(at: URL, withContentsOf: URL, options: NSFileVersion.AddingOptions) throws -> NSFileVersion

Creates a version of the file at the specified location.

### Accessing the Version Information

var url: URL

The URL identifying the location of the file associated with the file version object.

var localizedName: String?

The string containing the user-presentable name of the file version.

var localizedNameOfSavingComputer: String?

The user-presentable name of the computer on which the revision was saved.

var modificationDate: Date?

The modification date of the version.

var persistentIdentifier: any NSCoding

The identifier for this version of the file.

var isDiscardable: Bool

A Boolean value that specifies whether the system can delete the associated file at some future time.

### Handling Version Conflicts

var isConflict: Bool

A Boolean value indicating whether the contents of the version are in conflict with the contents of another version.

var isResolved: Bool

A Boolean value that indicates the version object is not in conflict (true) or is in conflict (false).

class func unresolvedConflictVersionsOfItem(at: URL) -> [NSFileVersion]?

Returns an array of version objects that are currently in conflict for the specified URL.

### Replacing and Deleting Versions

func replaceItem(at: URL, options: NSFileVersion.ReplacingOptions) throws -> URL

Replace the contents of the specified file with the contents of the current version’s file.

func remove() throws

Remove this version object and its associated file from the version store.

class func removeOtherVersionsOfItem(at: URL) throws

Removes all versions of a file, except the current one, from the version store.

### Constants

struct AddingOptions

Options for adding a new file version.

struct ReplacingOptions

Options for replacing a file version.

### Instance Properties

var hasLocalContents: Bool

var hasThumbnail: Bool

var originatorNameComponents: PersonNameComponents?

### Type Methods

class func getNonlocalVersionsOfItem(at: URL, completionHandler: ([NSFileVersion]?, (any Error)?) -> Void)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managed file access

class FileHandle

An object-oriented wrapper for a file descriptor.

class NSFileSecurity

A stub class that encapsulates security information about a file.

class FileWrapper

A representation of a node (a file, directory, or symbolic link) in the file system.

