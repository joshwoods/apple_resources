

- Foundation
- NSMutableArray
-  replaceObject(at:with:) 

Instance Method

# replaceObject(at:with:)

Replaces the object at `index` with `anObject`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceObject(
    at index: Int,
    with anObject: Any
)
```

## Parameters 

`index`  

The index of the object to be replaced. This value must not exceed the bounds of the array.

Important

Raises an `NSRangeException` if `index` is beyond the end of the array.

`anObject`  

The object with which to replace the object at index `index` in the array. This value must not be `nil`.

Important

Raises an `NSInvalidArgumentException` if `anObject` is `nil`.

## See Also

### Related Documentation

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the array.

func removeObject(at: Int)

Removes the object at `index` .

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

### Replacing Objects

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects in the receiving array at locations specified with the objects from a given array.

func replaceObjects(in: NSRange, withObjectsFrom: [Any], range: NSRange)

Replaces the objects in the receiving array specified by one given range with the objects in another array specified by another range.

func replaceObjects(in: NSRange, withObjectsFrom: [Any])

Replaces the objects in the receiving array specified by a given range with all of the objects from a given array.

func setArray([Any])

Sets the receiving array’s elements to those in another given array.

