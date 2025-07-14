

- Core Services
- Backup Core
-  CSBackupIsItemExcluded(\_:\_:) 

Function

# CSBackupIsItemExcluded(\_:\_:)

Returns a Boolean value indicating whether an item is currently excluded from the backup.

macOS 10.5+

``` source
func CSBackupIsItemExcluded(
    _ item: CFURL!,
    _ excludeByPath: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`item`  

The URL of the item.

`excludeByPath`  

If `true`, the item’s backup exclusion status applies to its location; if `false`, the item's backup exclusion status applies to itself, regardless of its location. See CSBackupSetItemExcluded(_:_:_:) for more information. Can be `NULL`.

## Return Value

`true` if the item or any of its ancestors are currently excluded from backup, `false` otherwise.

## See Also

### Managing an Item’s Backup Exclusion Status

func CSBackupSetItemExcluded(CFURL!, Bool, Bool) -> OSStatus

Includes or excludes an item from the backup.

