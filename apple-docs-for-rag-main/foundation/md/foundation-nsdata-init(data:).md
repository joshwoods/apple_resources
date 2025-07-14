

- Foundation
- NSData
-  init(data:) 

Initializer

# init(data:)

Initializes a data object with the contents of another data object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(data: Data)
```

## Parameters 

`data`  

A data object.

## Return Value

A data object initialized with the contents `data`.

## See Also

### Creating Data

init(bytes: UnsafeRawPointer?, length: Int)

Initializes a data object filled with a given number of bytes copied from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Initializes a data object filled with a given number of bytes of data from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?)

Initializes a data object filled with a given number of bytes of data from a given buffer, with a custom deallocator block.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, freeWhenDone: Bool)

Initializes a newly allocated data object by adding the given number of bytes from the given buffer.

