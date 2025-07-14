

- FSKit
- FSItem
- FSItem.Attributes
-  changeTime 

Instance Property

# changeTime

The item’s last-changed time.

macOS 15.4+

``` source
var changeTime: timespec { get set }
```

## Discussion

This property represents `ctime`, the last time the item’s metadata changed.

## See Also

### Working with time attributes

var accessTime: timespec

The item’s last-accessed time.

var modifyTime: timespec

The item’s last-modified time.

var birthTime: timespec

The item’s creation time.

var backupTime: timespec

The item’s last-backup time.

var addedTime: timespec

The item’s added time.

