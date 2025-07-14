

- Objective-C Runtime
- NSObject
-  copy() 

Instance Method

# copy()

Returns the object returned by `copy(with:)`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func copy() -> Any
```

## Return Value

The object returned by the NSCopying protocol method copy(with:),.

## Discussion

This is a convenience method for classes that adopt the NSCopying protocol. An exception is raised if there is no implementation for copy(with:).

`NSObject` does not itself support the NSCopying protocol. Subclasses must support the protocol and implement the copy(with:) method. A subclass version of the copy(with:) method should send the message to `super` first, to incorporate its implementation, unless the subclass descends directly from `NSObject`.

## See Also

### Creating, Copying, and Deallocating Objects

init()

Implemented by subclasses to initialize a new object (the receiver) immediately after memory for it has been allocated.

func mutableCopy() -> Any

Returns the object returned by `mutableCopy(with:)` where the zone is `nil`.

