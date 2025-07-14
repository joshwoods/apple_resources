

- Foundation
- NSFileVersion
-  persistentIdentifier 

Instance Property

# persistentIdentifier

The identifier for this version of the file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var persistentIdentifier: any NSCoding { get }
```

## Discussion

You can save the value of this property persistently and use it to recreate the version object later. When recreating the version object using the version(itemAt:forPersistentIdentifier:) method, the version object returned is equivalent to the current object.

## See Also

### Accessing the Version Information

var url: URL

The URL identifying the location of the file associated with the file version object.

var localizedName: String?

The string containing the user-presentable name of the file version.

var localizedNameOfSavingComputer: String?

The user-presentable name of the computer on which the revision was saved.

var modificationDate: Date?

The modification date of the version.

var isDiscardable: Bool

A Boolean value that specifies whether the system can delete the associated file at some future time.

