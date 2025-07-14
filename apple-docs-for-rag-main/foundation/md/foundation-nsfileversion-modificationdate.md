

- Foundation
- NSFileVersion
-  modificationDate 

Instance Property

# modificationDate

The modification date of the version.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var modificationDate: Date? { get }
```

## Discussion

If the version has been deleted, this value is `nil`.

## See Also

### Accessing the Version Information

var url: URL

The URL identifying the location of the file associated with the file version object.

var localizedName: String?

The string containing the user-presentable name of the file version.

var localizedNameOfSavingComputer: String?

The user-presentable name of the computer on which the revision was saved.

var persistentIdentifier: any NSCoding

The identifier for this version of the file.

var isDiscardable: Bool

A Boolean value that specifies whether the system can delete the associated file at some future time.

