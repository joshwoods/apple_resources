

- Foundation
- NSMutableArray
-  removeObject(identicalTo:in:) 

Instance Method

# removeObject(identicalTo:in:)

Removes all occurrences of `anObject` within the specified range in the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(
    identicalTo anObject: Any,
    in range: NSRange
)
```

## Parameters 

`anObject`  

The object to remove from the array within `aRange`.

`range`  

The range in the array from which to remove `anObject`.

Important

Raises an exception `NSRangeException` if `aRange` exceeds the bounds of the array.

## Discussion

This method determines a match by comparing the address of `anObject` to the addresses of objects in the receiver. If the array does not contain `anObject` within `aRange`, the method has no effect (although it does incur the overhead of searching the contents).

## See Also

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

func removeObjects(fromIndices: UnsafeMutablePointer&lt;Int>, numIndices: Int)

Removes the specified number of objects from the array, beginning at the specified index.

Deprecated

func removeObjects(in: [Any])

Removes from the receiving array the objects in another given array.

func removeObjects(in: NSRange)

Removes from the array each of the objects within a given range.

