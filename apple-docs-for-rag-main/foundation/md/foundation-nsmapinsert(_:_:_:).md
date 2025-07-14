

- Foundation
-  NSMapInsert(\_:\_:\_:) 

Function

# NSMapInsert(\_:\_:\_:)

Inserts a key-value pair into the specified table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSMapInsert(
    _ table: NSMapTable,
    _ key: UnsafeRawPointer?,
    _ value: UnsafeRawPointer?
)
```

## Discussion

Inserts `key` and `value` into `table`. If `key` matches a key already in `table`, `value` is retained and the previous value is released, using the `retain` and `release` callback functions that were specified when the table was created. Raises `NSInvalidArgumentException` if `key` is equal to the `notAKeyMarker` field of the table’s NSMapTableKeyCallBacks structure.

## See Also

### Related Documentation

func NSMapInsertIfAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Inserts a key-value pair into the specified table.

func NSMapRemove(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?)

Removes a key and corresponding value from the specified table.

func NSMapInsertKnownAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table if the pair had not been previously added.

### Functions

func NSAllMapTableKeys(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the keys in the specified map table.

func NSAllMapTableValues(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the values in the specified table.

func NSCompareMapTables(NSMapTable&lt;AnyObject, AnyObject>, NSMapTable&lt;AnyObject, AnyObject>) -> Bool

Compares the elements of two map tables for equality.

func NSCopyMapTableWithZone(NSMapTable&lt;AnyObject, AnyObject>, NSZone?) -> NSMapTable&lt;AnyObject, AnyObject>

Performs a shallow copy of the specified map table.

func NSCountMapTable(NSMapTable&lt;AnyObject, AnyObject>) -> Int

Returns the number of elements in a map table.

func NSCreateMapTable(NSMapTableKeyCallBacks, NSMapTableValueCallBacks, Int) -> NSMapTable&lt;AnyObject, AnyObject>

Creates a new map table in the default zone.

func NSCreateMapTableWithZone(NSMapTableKeyCallBacks, NSMapTableValueCallBacks, Int, NSZone?) -> NSMapTable&lt;AnyObject, AnyObject>

Creates a new map table in the specified zone.

func NSEndMapTableEnumeration(UnsafeMutablePointer&lt;NSMapEnumerator>)

Used when finished with an enumerator.

func NSEnumerateMapTable(NSMapTable&lt;AnyObject, AnyObject>) -> NSMapEnumerator

Creates an enumerator for the specified map table.

func NSFreeMapTable(NSMapTable&lt;AnyObject, AnyObject>)

Deletes the specified map table.

func NSMapGet(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Returns a map table value for the specified key.

func NSMapInsertIfAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Inserts a key-value pair into the specified table.

func NSMapInsertKnownAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table if the pair had not been previously added.

func NSMapMember(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> Bool

Indicates whether a given table contains a given key.

func NSMapRemove(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?)

Removes a key and corresponding value from the specified table.

