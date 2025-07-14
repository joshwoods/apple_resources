

- Swift
- UnsafeMutablePointer
-  initialize(repeating:count:) 

Instance Method

# initialize(repeating:count:)

Initializes this pointer’s memory with the specified number of consecutive copies of the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func initialize(
    repeating repeatedValue: Pointee,
    count: Int
)
```

## Parameters 

`repeatedValue`  

The instance to initialize this pointer’s memory with.

`count`  

The number of consecutive copies of `newValue` to initialize. `count` must not be negative.

## Discussion

The destination memory must be uninitialized or the pointer’s `Pointee` must be a trivial type. After a call to `initialize(repeating:count:)`, the memory referenced by this pointer is initialized.

