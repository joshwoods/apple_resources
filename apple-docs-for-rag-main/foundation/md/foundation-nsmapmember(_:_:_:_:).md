

- Foundation
-  NSMapMember(\_:\_:\_:\_:) 

Function

# NSMapMember(\_:\_:\_:\_:)

Indicates whether a given table contains a given key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSMapMember(
    _ table: NSMapTable,
    _ key: UnsafeRawPointer,
    _ originalKey: UnsafeMutablePointer?,
    _ value: UnsafeMutablePointer?
) -> Bool
```

## Return Value

true if `table` contains a key equal to `key`, otherwise false.

## Discussion

If `table` contains a key equal to `key`, `originalKey` is set to `key`, and `value` is set to the value that `table` maps to `key`.

## See Also

### Related Documentation

func NSNextMapEnumeratorPair(UnsafeMutablePointer&lt;NSMapEnumerator>, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> Bool

Returns a Boolean value that indicates whether the next map-table pair in the enumeration are set.

func NSAllMapTableValues(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the values in the specified table.

func NSMapGet(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Returns a map table value for the specified key.

func NSEnumerateMapTable(NSMapTable&lt;AnyObject, AnyObject>) -> NSMapEnumerator

Creates an enumerator for the specified map table.

func NSAllMapTableKeys(NSMapTable&lt;AnyObject, AnyObject>) -> [Any]

Returns all of the keys in the specified map table.

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

func NSMapInsert(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table.

func NSMapInsertIfAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Inserts a key-value pair into the specified table.

func NSMapInsertKnownAbsent(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?, UnsafeRawPointer?)

Inserts a key-value pair into the specified table if the pair had not been previously added.

func NSMapRemove(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?)

Removes a key and corresponding value from the specified table.

