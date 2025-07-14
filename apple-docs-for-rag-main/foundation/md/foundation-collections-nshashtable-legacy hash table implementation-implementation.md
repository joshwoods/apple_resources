

- Foundation
- Collections
- NSHashTable
-  Legacy Hash Table Implementation 

API Collection

# Legacy Hash Table Implementation

## Topics

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

func NSNextHashEnumeratorItem(UnsafeMutablePointer&lt;NSHashEnumerator>) -> UnsafeMutableRawPointer?

Returns the next hash-table element in the enumeration.

func NSResetHashTable(NSHashTable&lt;AnyObject>)

Deletes the elements of the specified hash table.

func NSStringFromHashTable(NSHashTable&lt;AnyObject>) -> String

Returns a string describing the hash table’s contents.

### Data Types

struct NSHashEnumerator

Allows successive elements of a hash table to be returned each time this structure is passed to NSNextHashEnumeratorItem(_:).

struct NSHashTableCallBacks

Defines a structure that contains the function pointers used to configure behavior of `NSHashTable` with respect to elements within a hash table.

typealias NSHashTableOptions

Components in a bit-field to specify the behavior of elements in an NSHashTable object.

### Constants

let NSIntegerHashCallBacks: NSHashTableCallBacks

For sets of `NSInteger`-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

let NSNonOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, hashed by address.

let NSNonRetainedObjectHashCallBacks: NSHashTableCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectHashCallBacks: NSHashTableCallBacks

For sets of objects (similar to `NSSet`).

let NSOwnedObjectIdentityHashCallBacks: NSHashTableCallBacks

For sets of objects, with transfer of ownership upon insertion, using pointer equality.

let NSOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, with transfer of ownership upon insertion.

let NSPointerToStructHashCallBacks: NSHashTableCallBacks

For sets of pointers to structs, when the first field of the struct is `int`-sized.

## See Also

### Deprecated

