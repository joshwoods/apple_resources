

- Swift
- UnsafeMutablePointer
-  pointee 

Instance Property

# pointee

Reads or updates the instance referenced by this pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pointee: Pointee { get nonmutating set }
```

## Discussion

When reading from the `pointee` property, the instance referenced by this pointer must already be initialized. When `pointee` is used as the left side of an assignment, the instance is updated. The instance must be initialized or this pointer’s `Pointee` type must be a trivial type.

Uninitialized memory cannot be initialized to a nontrivial type using `pointee`. Instead, use an initializing method, such as `initialize(to:)`.

