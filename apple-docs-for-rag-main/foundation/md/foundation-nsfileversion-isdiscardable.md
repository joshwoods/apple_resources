

- Foundation
- NSFileVersion
-  isDiscardable 

Instance Property

# isDiscardable

A Boolean value that specifies whether the system can delete the associated file at some future time.

macOS 10.7+

``` source
var isDiscardable: Bool { get set }
```

## Discussion

Marking a file version as discardable gives the system the flexibility to reclaim the space, occupied by the associated file, at some future time. Do not, however, depend on the file being discarded.

After setting this property to true, do not set this property to false again. Doing so causes the system to raise an exception. In addition, if you set this property to true for the version of the file returned by the currentVersionOfItem(at:) method, the system raises an exception.

## See Also

### Related Documentation

class func removeOtherVersionsOfItem(at: URL) throws

Removes all versions of a file, except the current one, from the version store.

func remove() throws

Remove this version object and its associated file from the version store.

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

