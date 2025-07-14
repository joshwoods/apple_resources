

- Swift
- ManagedBuffer
-  header 

Instance Property

# header

The stored `Header` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
final var header: Header
```

## Discussion

During instance creation, in particular during `ManagedBuffer.create`’s call to initialize, `ManagedBuffer`’s `header` property is as-yet uninitialized, and therefore reading the `header` property during `ManagedBuffer.create` is undefined.

