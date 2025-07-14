

- Swift
- ManagedBufferPointer
-  init(unsafeBufferObject:) 

Initializer

# init(unsafeBufferObject:)

Manage the given `buffer`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(unsafeBufferObject buffer: AnyObject)
```

## Discussion

Precondition

`buffer` is an instance of a non-`@objc` class whose `deinit` destroys its stored `Header` and any constructed `Element`s.

## See Also

### Creating a Buffer

init(bufferClass: AnyClass, minimumCapacity: Int, makingHeaderWith: (AnyObject, (AnyObject) -> Int) throws -> Header) rethrows

Create with new storage containing an initial `Header` and space for at least `minimumCapacity` `element`s.

