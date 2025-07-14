

- Foundation
- NSSet
-  addingObjects(from:) 

Instance Method

# addingObjects(from:)

Returns a new set formed by adding the objects in a given set to the receiving set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addingObjects(from other: Set) -> Set
```

## Parameters 

`other`  

The set of objects to add to the receiving set.

## Return Value

A new set formed by adding the objects in `other` to the receiving set.

## See Also

### Creating a Set

convenience init(object: Any)

Creates and returns a set that contains a single given object.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

func adding(Any) -> Set&lt;AnyHashable>

Returns a new set formed by adding a given object to the receiving set.

func addingObjects(from: [Any]) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given array to the receiving set.

