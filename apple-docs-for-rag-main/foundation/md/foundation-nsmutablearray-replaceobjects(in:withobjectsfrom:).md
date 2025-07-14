

- Foundation
- NSMutableArray
-  replaceObjects(in:withObjectsFrom:) 

Instance Method

# replaceObjects(in:withObjectsFrom:)

Replaces the objects in the receiving array specified by a given range with all of the objects from a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceObjects(
    in range: NSRange,
    withObjectsFrom otherArray: [Any]
)
```

## Parameters 

`range`  

The range of objects to be replaced in (or removed from) the receiving array.

`otherArray`  

The array of objects from which to select replacements for the objects in `aRange`.

## Discussion

If `otherArray` has fewer objects than are specified by `aRange`, the extra objects in the receiving array are removed. If `otherArray` has more objects than are specified by `aRange`, the extra objects from `otherArray` are inserted into the receiving array.

## See Also

### Related Documentation

func removeObject(at: Int)

Removes the object at `index` .

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

### Replacing Objects

func replaceObject(at: Int, with: Any)

Replaces the object at `index` with `anObject`.

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects in the receiving array at locations specified with the objects from a given array.

func replaceObjects(in: NSRange, withObjectsFrom: [Any], range: NSRange)

Replaces the objects in the receiving array specified by one given range with the objects in another array specified by another range.

func setArray([Any])

Sets the receiving array’s elements to those in another given array.

