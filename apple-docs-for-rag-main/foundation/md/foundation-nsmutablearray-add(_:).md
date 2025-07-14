

- Foundation
- NSMutableArray
-  add(\_:) 

Instance Method

# add(\_:)

Inserts a given object at the end of the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(_ anObject: Any)
```

## Parameters 

`anObject`  

The object to add to the end of the array’s content. This value must not be `nil`.

Important

Raises an `NSInvalidArgumentException` if `anObject` is `nil`.

## See Also

### Related Documentation

func remove(Any)

Removes all occurrences in the array of a given object.

func setArray([Any])

Sets the receiving array’s elements to those in another given array.

### Adding Objects

func addObjects(from: [Any])

Adds the objects contained in another given array to the end of the receiving array’s content.

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

func insert([Any], at: IndexSet)

Inserts the objects in the provided array into the receiving array at the specified indexes.

