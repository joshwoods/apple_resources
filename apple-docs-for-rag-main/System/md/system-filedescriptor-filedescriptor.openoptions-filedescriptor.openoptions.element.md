

- System
- FileDescriptor
- FileDescriptor.OpenOptions
-  FileDescriptor.OpenOptions.Element 

Type Alias

# FileDescriptor.OpenOptions.Element

The element type of the option set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
typealias Element = FileDescriptor.OpenOptions
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

