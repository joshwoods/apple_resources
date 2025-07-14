

- Swift
- UnsafeMutableBufferPointer
-  initialize(repeating:) 

Instance Method

# initialize(repeating:)

Initializes every element in this buffer’s memory to a copy of the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func initialize(repeating repeatedValue: Element)
```

## Parameters 

`repeatedValue`  

The instance to initialize this buffer’s memory with.

## Discussion

The destination memory must be uninitialized or the buffer’s `Element` must be a trivial type. After a call to `initialize(repeating:)`, the entire region of memory referenced by this buffer is initialized.

