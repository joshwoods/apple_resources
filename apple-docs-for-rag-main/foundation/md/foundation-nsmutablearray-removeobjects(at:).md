

- Foundation
- NSMutableArray
-  removeObjects(at:) 

Instance Method

# removeObjects(at:)

Removes the objects at the specified indexes from the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObjects(at indexes: IndexSet)
```

## Parameters 

`indexes`  

The indexes of the objects to remove from the array. The locations specified by `indexes` must lie within the bounds of the array.

## Discussion

This method is similar to removeObject(at:), but allows you to efficiently remove multiple objects with a single operation. `indexes` specifies the locations of objects to be removed given the state of the array when the method is invoked, as illustrated in the following example:

```
NSMutableArray *array = [NSMutableArray arrayWithObjects: @"one", @"a", @"two", @"b", @"three", @"four", nil];
NSMutableIndexSet *indexes = [NSMutableIndexSet indexSetWithIndex:1];
[indexes addIndex:3];
[array removeObjectsAtIndexes:indexes];
NSLog(@"array: %@", array);

// Output: array: (one, two, three, four)
```

If `indexes` is `nil`, this method raises an exception.

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

