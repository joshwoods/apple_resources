

- Foundation
- NSMutableArray
-  setArray(\_:) 

Instance Method

# setArray(\_:)

Sets the receiving array’s elements to those in another given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setArray(_ otherArray: [Any])
```

## Parameters 

`otherArray`  

The array of objects with which to replace the receiving array’s content.

## See Also

### Related Documentation

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

func addObjects(from: [Any])

Adds the objects contained in another given array to the end of the receiving array’s content.

### Replacing Objects

func replaceObject(at: Int, with: Any)

Replaces the object at `index` with `anObject`.

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects in the receiving array at locations specified with the objects from a given array.

func replaceObjects(in: NSRange, withObjectsFrom: [Any], range: NSRange)

Replaces the objects in the receiving array specified by one given range with the objects in another array specified by another range.

func replaceObjects(in: NSRange, withObjectsFrom: [Any])

Replaces the objects in the receiving array specified by a given range with all of the objects from a given array.

