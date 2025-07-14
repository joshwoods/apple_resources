

- Foundation
- NSMutableArray
-  removeObjects(fromIndices:numIndices:) Deprecated

Instance Method

# removeObjects(fromIndices:numIndices:)

Removes the specified number of objects from the array, beginning at the specified index.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func removeObjects(
    fromIndices indices: UnsafeMutablePointer,
    numIndices cnt: Int
)
```

Deprecated

Do not use this method, use removeObjects(at:) instead.

## Parameters 

`indices`  

A C array of the indices of the objects to remove from the receiving array.

`cnt`  

The number of objects to remove from the receiving array.

## Discussion

This method is similar to removeObject(at:), but it allows you to efficiently remove multiple objects with a single operation. If you sort the list of indexes in ascending order, you will improve the speed of this operation.

This method cannot be sent to a remote object with distributed objects.

### Special Considerations

This deprecated method uses a C array of indices. The removeObjects(at:) method uses an NSIndexSet which provides a more efficient way of indexing into an array.

## See Also

### Related Documentation

init(capacity: Int)

Returns an array, initialized with enough memory to initially hold a given number of objects.

### Removing Objects

func removeAllObjects()

Empties the array of all its elements.

func removeLastObject()

Removes the object with the highest-valued index in the array

func remove(Any)

Removes all occurrences in the array of a given object.

func remove(Any, in: NSRange)

Removes all occurrences within a specified range in the array of a given object.

func removeObject(at: Int)

Removes the object at `index` .

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the array.

func removeObject(identicalTo: Any)

Removes all occurrences of a given object in the array.

func removeObject(identicalTo: Any, in: NSRange)

Removes all occurrences of `anObject` within the specified range in the array.

func removeObjects(in: [Any])

Removes from the receiving array the objects in another given array.

func removeObjects(in: NSRange)

Removes from the array each of the objects within a given range.

