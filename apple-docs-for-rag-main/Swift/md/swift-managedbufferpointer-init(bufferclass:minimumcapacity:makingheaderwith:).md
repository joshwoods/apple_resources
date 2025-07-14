

- Swift
- ManagedBufferPointer
-  init(bufferClass:minimumCapacity:makingHeaderWith:) 

Initializer

# init(bufferClass:minimumCapacity:makingHeaderWith:)

Create with new storage containing an initial `Header` and space for at least `minimumCapacity` `element`s.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bufferClass: AnyClass,
    minimumCapacity: Int,
    makingHeaderWith factory: (AnyObject, (AnyObject) -> Int) throws -> Header
) rethrows
```

## Parameters 

`bufferClass`  

The class of the object used for storage.

`minimumCapacity`  

The minimum number of `Element`s that must be able to be stored in the new buffer.

`factory`  

A function that produces the initial `Header` instance stored in the buffer, given the `buffer` object and a function that can be called on it to get the actual number of allocated elements.

## Discussion

Precondition

`minimumCapacity >= 0`, and the type indicated by `bufferClass` is a non-`@objc` class with no declared stored properties. The `deinit` of `bufferClass` must destroy its stored `Header` and any constructed `Element`s.

## See Also

### Creating a Buffer

init(unsafeBufferObject: AnyObject)

Manage the given `buffer`.

