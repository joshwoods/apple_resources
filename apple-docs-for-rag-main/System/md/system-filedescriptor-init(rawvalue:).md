

- System
- FileDescriptor
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a strongly-typed file handle from a raw C file handle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(rawValue: CInt)
```

## See Also

### Creating a File Descriptor

let rawValue: CInt

The raw C file handle.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

