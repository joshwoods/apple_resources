

- Foundation
-  NSHashInsert(\_:\_:) 

Function

# NSHashInsert(\_:\_:)

Adds an element to the specified hash table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSHashInsert(
    _ table: NSHashTable,
    _ pointer: UnsafeRawPointer?
)
```

## Discussion

Inserts `pointer`, which must not be `NULL`, into `table`. If `pointer` matches an item already in the table, the previous pointer is released using the `release` callback function that was specified when the table was created.

## See Also

### Related Documentation

func NSHashInsertKnownAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Adds an element to the specified hash table.

func NSHashRemove(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Removes an element from the specified hash table.

func NSHashInsertIfAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Adds an element to the specified hash table only if the table does not already contain the element.

### Functions

func NSAllHashTableObjects(NSHashTable&lt;AnyObject>) -> [Any]

Returns all of the elements in the specified hash table.

func NSCompareHashTables(NSHashTable&lt;AnyObject>, NSHashTable&lt;AnyObject>) -> Bool

Returns a Boolean value that indicates whether the elements of two hash tables are equal.

func NSCopyHashTableWithZone(NSHashTable&lt;AnyObject>, NSZone?) -> NSHashTable&lt;AnyObject>

Performs a shallow copy of the specified hash table.

func NSCountHashTable(NSHashTable&lt;AnyObject>) -> Int

Returns the number of elements in a hash table.

func NSCreateHashTable(NSHashTableCallBacks, Int) -> NSHashTable&lt;AnyObject>

Creates and returns a new hash table.

func NSCreateHashTableWithZone(NSHashTableCallBacks, Int, NSZone?) -> NSHashTable&lt;AnyObject>

Creates a new hash table in a given zone.

func NSEndHashTableEnumeration(UnsafeMutablePointer&lt;NSHashEnumerator>)

Used when finished with an enumerator.

func NSEnumerateHashTable(NSHashTable&lt;AnyObject>) -> NSHashEnumerator

Creates an enumerator for the specified hash table.

func NSFreeHashTable(NSHashTable&lt;AnyObject>)

Deletes the specified hash table.

func NSHashGet(NSHashTable&lt;AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer

Returns an element of the hash table.

func NSHashInsertIfAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Adds an element to the specified hash table only if the table does not already contain the element.

func NSHashInsertKnownAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Adds an element to the specified hash table.

func NSHashRemove(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Removes an element from the specified hash table.

func NSNextHashEnumeratorItem(UnsafeMutablePointer&lt;NSHashEnumerator>) -> UnsafeMutableRawPointer?

Returns the next hash-table element in the enumeration.

func NSResetHashTable(NSHashTable&lt;AnyObject>)

Deletes the elements of the specified hash table.

