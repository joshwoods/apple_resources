

- FSKit
- FSItem
- FSItem.Attributes
-  modifyTime 

Instance Property

# modifyTime

The item’s last-modified time.

macOS 15.4+

``` source
var modifyTime: timespec { get set }
```

## Discussion

This property represents `mtime`, the last time the item’s contents changed.

## See Also

### Working with time attributes

var accessTime: timespec

The item’s last-accessed time.

var changeTime: timespec

The item’s last-changed time.

var birthTime: timespec

The item’s creation time.

var backupTime: timespec

The item’s last-backup time.

var addedTime: timespec

The item’s added time.

