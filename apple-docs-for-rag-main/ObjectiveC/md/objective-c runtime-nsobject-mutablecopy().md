

- Objective-C Runtime
- NSObject
-  mutableCopy() 

Instance Method

# mutableCopy()

Returns the object returned by `mutableCopy(with:)` where the zone is `nil`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func mutableCopy() -> Any
```

## Return Value

The object returned by the NSMutableCopying protocol method mutableCopy(with:), where the zone is `nil`.

## Discussion

This is a convenience method for classes that adopt the NSMutableCopying protocol. An exception is raised if there is no implementation for mutableCopy(with:).

## See Also

### Creating, Copying, and Deallocating Objects

init()

Implemented by subclasses to initialize a new object (the receiver) immediately after memory for it has been allocated.

func copy() -> Any

Returns the object returned by `copy(with:)`.

