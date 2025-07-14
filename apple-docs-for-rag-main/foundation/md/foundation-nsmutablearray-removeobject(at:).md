

- Foundation
- NSMutableArray
-  removeObject(at:) 

Instance Method

# removeObject(at:)

Removes the object at `index` .

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(at index: Int)
```

## Parameters 

`index`  

The index from which to remove the object in the array. The value must not exceed the bounds of the array.

Important

Raises an exception `NSRangeException` if `index` is beyond the end of the array.

## Discussion

To fill the gap, all elements beyond `index` are moved by subtracting 1 from their index.

## See Also

### Related Documentation

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

### Removing Objects

func removeAllObjects()

Empties the array of all its elements.

func removeLastObject()

Removes the object with the highest-valued index in the array

func remove(Any)

Removes all occurrences in the array of a given object.

func remove(Any, in: NSRange)

Removes all occurrences within a specified range in the array of a given object.

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the array.

func removeObject(identicalTo: Any)

Removes all occurrences of a given object in the array.

func removeObject(identicalTo: Any, in: NSRange)

Removes all occurrences of `anObject` within the specified range in the array.

func removeObjects(fromIndices: UnsafeMutablePointer&lt;Int>, numIndices: Int)

Removes the specified number of objects from the array, beginning at the specified index.

Deprecated

func removeObjects(in: [Any])

Removes from the receiving array the objects in another given array.

func removeObjects(in: NSRange)

Removes from the array each of the objects within a given range.

