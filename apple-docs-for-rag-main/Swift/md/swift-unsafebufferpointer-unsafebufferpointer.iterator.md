

- Swift
- UnsafeBufferPointer
-  UnsafeBufferPointer.Iterator 

Structure

# UnsafeBufferPointer.Iterator

An iterator for the elements in the buffer referenced by an `UnsafeBufferPointer` or `UnsafeMutableBufferPointer` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

## Topics

### Default Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- IteratorProtocol

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

