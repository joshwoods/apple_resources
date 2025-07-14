

- Foundation
- NSFileVersion
-  localizedNameOfSavingComputer 

Instance Property

# localizedNameOfSavingComputer

The user-presentable name of the computer on which the revision was saved.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizedNameOfSavingComputer: String? { get }
```

## Discussion

If the current revision has been deleted from disk, or if no computer name was recorded, the value in this property is `nil`. The computer name is guaranteed to be recorded only when the current version is in conflict with another version. The version object does not track changes to the computer name itself. Thus, if the computer name changed, the value in this string might be an old value.

## See Also

### Accessing the Version Information

var url: URL

The URL identifying the location of the file associated with the file version object.

var localizedName: String?

The string containing the user-presentable name of the file version.

var modificationDate: Date?

The modification date of the version.

var persistentIdentifier: any NSCoding

The identifier for this version of the file.

var isDiscardable: Bool

A Boolean value that specifies whether the system can delete the associated file at some future time.

