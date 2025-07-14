

- Foundation
- NSMutableArray
-  replaceObjects(at:with:) 

Instance Method

# replaceObjects(at:with:)

Replaces the objects in the receiving array at locations specified with the objects from a given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceObjects(
    at indexes: IndexSet,
    with objects: [Any]
)
```

## Parameters 

`indexes`  

The indexes of the objects to be replaced.

`objects`  

The objects with which to replace the objects in the receiving array at the indexes specified by `indexes`. The count of locations in `indexes` must equal the count of `objects`.

## Discussion

The indexes in `indexes` are used in the same order as the objects in `objects`.

If `objects` or `indexes` is `nil`, this method raises an exception.

## See Also

### Related Documentation

func removeObject(at: Int)

Removes the object at `index` .

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

### Replacing Objects

func replaceObject(at: Int, with: Any)

Replaces the object at `index` with `anObject`.

func replaceObjects(in: NSRange, withObjectsFrom: [Any], range: NSRange)

Replaces the objects in the receiving array specified by one given range with the objects in another array specified by another range.

func replaceObjects(in: NSRange, withObjectsFrom: [Any])

Replaces the objects in the receiving array specified by a given range with all of the objects from a given array.

func setArray([Any])

Sets the receiving array’s elements to those in another given array.

