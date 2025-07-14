

- System
- FileDescriptor
-  pipe() 

Type Method

# pipe()

Creates a unidirectional data channel, which can be used for interprocess communication.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
static func pipe() throws -> (readEnd: FileDescriptor, writeEnd: FileDescriptor)
```

## Return Value

The pair of file descriptors.

## Discussion

The corresponding C function is `pipe`.

