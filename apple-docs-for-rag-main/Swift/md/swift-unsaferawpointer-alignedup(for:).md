

- Swift
- UnsafeRawPointer
-  alignedUp(for:) 

Instance Method

# alignedUp(for:)

Obtain the next pointer properly aligned to store a value of type `T`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func alignedUp(for type: T.Type) -> UnsafeRawPointer where T : ~Copyable
```

## Parameters 

`type`  

The type to be stored at the returned address.

## Return Value

A pointer properly aligned to store a value of type `T`.

## Discussion

If `self` is properly aligned for accessing `T`, this function returns `self`.

