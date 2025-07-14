

- Foundation
-  NSNextHashEnumeratorItem(\_:) 

Function

# NSNextHashEnumeratorItem(\_:)

Returns the next hash-table element in the enumeration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSNextHashEnumeratorItem(_ enumerator: UnsafeMutablePointer) -> UnsafeMutableRawPointer?
```

## Return Value

The next element in the table that `enumerator` is associated with, or `NULL` if `enumerator` has already iterated over all the elements.

## See Also

### Related Documentation

func NSEnumerateHashTable(NSHashTable&lt;AnyObject>) -> NSHashEnumerator

Creates an enumerator for the specified hash table.

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

func NSHashInsert(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Adds an element to the specified hash table.

func NSHashInsertIfAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?) -> UnsafeMutableRawPointer?

Adds an element to the specified hash table only if the table does not already contain the element.

func NSHashInsertKnownAbsent(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Adds an element to the specified hash table.

func NSHashRemove(NSHashTable&lt;AnyObject>, UnsafeRawPointer?)

Removes an element from the specified hash table.

func NSResetHashTable(NSHashTable&lt;AnyObject>)

Deletes the elements of the specified hash table.

