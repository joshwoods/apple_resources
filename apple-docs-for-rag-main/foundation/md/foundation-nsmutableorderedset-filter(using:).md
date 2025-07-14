

- Foundation
- NSMutableOrderedSet
-  filter(using:) 

Instance Method

# filter(using:)

Evaluates a given predicate against the mutable ordered set’s content and leaves only objects that match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filter(using p: NSPredicate)
```

## Parameters 

`p`  

The predicate to evaluate against the set’s elements.

## See Also

### Related Documentation

func filtered(using: NSPredicate) -> NSOrderedSet

Evaluates a given predicate against each object in the receiving ordered set and returns a new ordered set containing the objects for which the predicate returns true.

### Adding, Removing, and Reordering Entries

func add(Any)

Appends a given object to the end of the mutable ordered set, if it is not already a member.

func add(UnsafePointer&lt;AnyObject>?, count: Int)

Appends the given number of objects from a given C array to the end of the mutable ordered set.

func addObjects(from: [Any])

Appends to the end of the mutable ordered set each object contained in a given array that is not already a member.

func insert(Any, at: Int)

Inserts the given object at the specified index of the mutable ordered set, if it is not already a member.

func insert([Any], at: IndexSet)

Inserts the objects in the array at the specified indexes.

func remove(Any)

Removes a given object from the mutable ordered set.

func removeObject(at: Int)

Removes a the object at the specified index from the mutable ordered set.

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the mutable ordered set.

func removeObjects(in: [Any])

Removes the objects in the array from the mutable ordered set.

func removeObjects(in: NSRange)

Removes from the mutable ordered set each of the objects within a given range.

func removeAllObjects()

Removes all the objects from the mutable ordered set.

func replaceObject(at: Int, with: Any)

Replaces the object at the specified index with the new object.

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects at the specified indexes with the new objects.

func replaceObjects(in: NSRange, with: UnsafePointer&lt;AnyObject>?, count: Int)

Replaces the objects in the receiving mutable ordered set at the range with the specified number of objects from a given C array.

func setObject(Any, at: Int)

Appends or replaces the object at the specified index.

