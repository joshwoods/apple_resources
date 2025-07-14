

- Foundation
-  NSCopyMapTableWithZone(\_:\_:) 

Function

# NSCopyMapTableWithZone(\_:\_:)

Performs a shallow copy of the specified map table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSCopyMapTableWithZone(
    _ table: NSMapTable,
    _ zone: NSZone?
) -> NSMapTable
```

## Return Value

A pointer to a new copy of `table`, created in `zone` and containing pointers to the keys and values of `table`.

## Discussion

If `zone` is `NULL`, the new table is created in the default zone.

The new table adopts the callback functions of `table` and calls the `hash` and `retain` callback functions as appropriate when inserting elements into the new table.

## See Also

### Related Documentation

func NSCreateMapTableWithZone(NSMapTableKeyCallBacks, NSMapTableValueCallBacks, Int, NSZone?) -> NSMapTable&lt;AnyObject, AnyObject>

Creates a new map table in the specified zone.

func NSCreateMapTable(NSMapTableKeyCallBacks, NSMapTableValueCallBacks, Int) -> NSMapTable&lt;AnyObject, AnyObject>

Creates a new map table in the default zone.

struct NSMapTableValueCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to value elements within a map table.

struct NSMapTableKeyCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to key elements within a map table.

### Functions

func NSAllMapTableKeys(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the keys in the specified map table.

func NSAllMapTableValues(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the values in the specified table.

func NSCompareMapTables(NSMapTable&lt;AnyObject, AnyObject>, NSMapTable&lt;AnyObject, AnyObject>) -> Bool

Compares the elements of two map tables for equality.

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

func NSMapInsert(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table.

func NSMapInsertIfAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Inserts a key-value pair into the specified table.

func NSMapInsertKnownAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table if the pair had not been previously added.

func NSMapMember(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> Bool

Indicates whether a given table contains a given key.

func NSMapRemove(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?)

Removes a key and corresponding value from the specified table.

