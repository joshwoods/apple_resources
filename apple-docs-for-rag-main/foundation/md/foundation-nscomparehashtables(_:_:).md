

- Foundation
-  NSCompareHashTables(\_:\_:) 

Function

# NSCompareHashTables(\_:\_:)

Returns a Boolean value that indicates whether the elements of two hash tables are equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSCompareHashTables(
    _ table1: NSHashTable,
    _ table2: NSHashTable
) -> Bool
```

## Return Value

true if the two hash tables are equal—that is, if each element of `table1` is in `table2` and the two tables are the same size, otherwise false.

## See Also

### Related Documentation

func NSCreateHashTable(NSHashTableCallBacks, Int) -> NSHashTable&lt;AnyObject>

Creates and returns a new hash table.

func NSCreateHashTableWithZone(NSHashTableCallBacks, Int, NSZone?) -> NSHashTable&lt;AnyObject>

Creates a new hash table in a given zone.

### Functions

func NSAllHashTableObjects(NSHashTable&lt;AnyObject>) -> [Any]

Returns all of the elements in the specified hash table.

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

func NSHashInsert(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Adds an element to the specified hash table.

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

