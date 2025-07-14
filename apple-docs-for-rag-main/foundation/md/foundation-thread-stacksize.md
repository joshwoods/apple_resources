

- Foundation
- Thread
-  stackSize 

Instance Property

# stackSize

The stack size of the receiver, in bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var stackSize: Int { get set }
```

## Discussion

This value must be in bytes and a multiple of 4KB.

To change the stack size, you must set this property before starting your thread. Setting the stack size after the thread has started changes the attribute size (which is reflected by the stackSize method), but it does not affect the actual number of pages set aside for the thread.

## See Also

### Working with Thread Properties

var threadDictionary: NSMutableDictionary

The thread object’s dictionary.

let NSAssertionHandlerKey: String

var name: String?

The name of the receiver.

