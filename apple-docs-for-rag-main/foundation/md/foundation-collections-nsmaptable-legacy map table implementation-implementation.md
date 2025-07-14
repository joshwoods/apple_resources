

- Foundation
- Collections
- NSMapTable
-  Legacy Map Table Implementation 

API Collection

# Legacy Map Table Implementation

## Topics

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

func NSMapMember(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> Bool

Indicates whether a given table contains a given key.

func NSMapRemove(NSMapTable&lt;AnyObject, AnyObject>, UnsafeRawPointer?)

Removes a key and corresponding value from the specified table.

func NSNextMapEnumeratorPair(UnsafeMutablePointer&lt;NSMapEnumerator>, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>?) -> Bool

Returns a Boolean value that indicates whether the next map-table pair in the enumeration are set.

func NSResetMapTable(NSMapTable&lt;AnyObject, AnyObject>)

Deletes the elements of the specified map table.

func NSStringFromMapTable(NSMapTable&lt;AnyObject, AnyObject>) -> String

Returns a string describing the map table’s contents.

### Data Types

struct NSMapEnumerator

Allows successive elements of a map table to be returned each time this structure is passed to NSNextMapEnumeratorPair(_:_:_:).

NSMapTable

The opaque data type used by the functions described in Managing Map Tables.

struct NSMapTableKeyCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to key elements within a map table.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

struct NSMapTableValueCallBacks

The function pointers used to configure behavior of `NSMapTable` with respect to value elements within a map table.

### Constants

let NSIntegerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

let NSIntMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

Deprecated

let NSNonOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers not freed.

let NSNonOwnedPointerOrNullMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers not freed, or `NULL`.

let NSNonRetainedObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are objects.

let NSOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers, with transfer of ownership upon insertion.

### Constants

let NSIntegerMapValueCallBacks: NSMapTableValueCallBacks

For values that are pointer-sized quantities, (for example, `int`, `long`, or `unichar`).

let NSIntMapValueCallBacks: NSMapTableValueCallBacks

For values that are pointer-sized quantities, (for example, `int`, `long`, or `unichar`).

Deprecated

let NSNonOwnedPointerMapValueCallBacks: NSMapTableValueCallBacks

For values that are not owned pointers.

let NSOwnedPointerMapValueCallBacks: NSMapTableValueCallBacks

For values that are owned pointers.

let NSNonRetainedObjectMapValueCallBacks: NSMapTableValueCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectMapValueCallBacks: NSMapTableValueCallBacks

For values that are objects.

## See Also

### Deprecated

