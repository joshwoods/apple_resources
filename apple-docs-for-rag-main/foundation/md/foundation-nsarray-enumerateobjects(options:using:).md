

- Foundation
- NSArray
-  enumerateObjects(options:using:) 

Instance Method

# enumerateObjects(options:using:)

Executes a given closure or block using each object in the array with the specified options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateObjects(
    options opts: NSEnumerationOptions = [],
    using block: (Any, Int, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`opts`  

The options for the enumeration. For possible values, see NSEnumerationOptions.

`block`  

A closure or block to execute for each object in the array, taking three arguments:

- The object.

- The index of the object in the array.

- A reference to a Boolean value, which the closure can set to true in order to stop further enumeration of the array. If a closure stops further enumeration, that closure continues to run until it’s finished. When the concurrent enumeration option is specified, enumeration stops after all of the currently running closures finish.

## Discussion

This method executes synchronously. By default, the enumeration starts with the first object and continues serially through the array to the last object. You can specify concurrent and/or reverse as enumeration options to modify this behavior.

## See Also

### Sending Messages to Elements

func enumerateObjects((Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given closure or block using each object in the array, starting with the first object and continuing through the array to the last object.

func enumerateObjects(at: IndexSet, options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using the objects in the array at the specified indexes.

