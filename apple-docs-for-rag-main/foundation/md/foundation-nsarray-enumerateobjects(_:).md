

- Foundation
- NSArray
-  enumerateObjects(\_:) 

Instance Method

# enumerateObjects(\_:)

Executes a given closure or block using each object in the array, starting with the first object and continuing through the array to the last object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateObjects(_ block: (Any, Int, UnsafeMutablePointer) -> Void)
```

## Parameters 

`block`  

A closure or block to execute for each object in the array, taking three arguments:

- The object.

- The index of the object in the array.

- A reference to a Boolean value, which the closure can set to true in order to stop further enumeration of the array. If a closure stops further enumeration, that closure continues to run until it’s finished.

## Discussion

This method executes synchronously. Values allocated within the block are deallocated after the block is executed.

## See Also

### Sending Messages to Elements

func enumerateObjects(options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given closure or block using each object in the array with the specified options.

func enumerateObjects(at: IndexSet, options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using the objects in the array at the specified indexes.

