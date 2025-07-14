

- FSKit
- FSItem
- FSItem.Attributes
-  addedTime 

Instance Property

# addedTime

The item’s added time.

macOS 15.4+

``` source
var addedTime: timespec { get set }
```

## Discussion

This property represents the time the file system added the item to its parent directory.

## See Also

### Working with time attributes

var accessTime: timespec

The item’s last-accessed time.

var modifyTime: timespec

The item’s last-modified time.

var changeTime: timespec

The item’s last-changed time.

var birthTime: timespec

The item’s creation time.

var backupTime: timespec

The item’s last-backup time.

