

- Foundation
- NSSet
-  adding(\_:) 

Instance Method

# adding(\_:)

Returns a new set formed by adding a given object to the receiving set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func adding(_ anObject: Any) -> Set
```

## Parameters 

`anObject`  

The object to add to the set.

## Return Value

A new set formed by adding `anObject` to the receiving set.

## See Also

### Creating a Set

convenience init(object: Any)

Creates and returns a set that contains a single given object.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

func addingObjects(from: Set&lt;AnyHashable>) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given set to the receiving set.

func addingObjects(from: [Any]) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given array to the receiving set.

