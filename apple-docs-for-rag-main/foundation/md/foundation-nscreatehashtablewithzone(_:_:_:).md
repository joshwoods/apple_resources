

- Foundation
-  NSCreateHashTableWithZone(\_:\_:\_:) 

Function

# NSCreateHashTableWithZone(\_:\_:\_:)

Creates a new hash table in a given zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSCreateHashTableWithZone(
    _ callBacks: NSHashTableCallBacks,
    _ capacity: Int,
    _ zone: NSZone?
) -> NSHashTable
```

## Return Value

A pointer to a new hash table created in the specified zone. If `zone` is `NULL`, the hash table is created in the default zone.

## Discussion

The table’s size is dependent on (but generally not equal to) `capacity`. If `capacity` is 0, a small hash table is created. The NSHashTableCallBacks structure `callBacks` has five pointers to functions, with the following defaults: pointer hashing, if `hash` is `NULL`; pointer equality, if `isEqual` is `NULL`; no callback upon adding an element, if `retain` is `NULL`; no callback upon removing an element, if `release` is `NULL`; and a function returning a pointer’s hexadecimal value as a string, if `describe` is `NULL`. The hashing function must be defined such that if two data elements are equal, as defined by the comparison function, the values produced by hashing on these elements must also be equal. Also, data elements must remain invariant if the value of the hashing function depends on them; for example, if the hashing function operates directly on the characters of a string, that string can’t change.

## See Also

### Related Documentation

func NSCreateHashTable(NSHashTableCallBacks, Int) -> NSHashTable&lt;AnyObject>

Creates and returns a new hash table.

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

