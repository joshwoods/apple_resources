

- Foundation
- NSSet
-  init(object:) 

Initializer

# init(object:)

Creates and returns a set that contains a single given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(object: Any)
```

## Parameters 

`object`  

The object to add to the new set. `object` receives a retain message after being added to the set.

## Return Value

A new set that contains a single member, `object`.

## See Also

### Creating a Set

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

func adding(Any) -> Set&lt;AnyHashable>

Returns a new set formed by adding a given object to the receiving set.

func addingObjects(from: Set&lt;AnyHashable>) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given set to the receiving set.

func addingObjects(from: [Any]) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given array to the receiving set.

