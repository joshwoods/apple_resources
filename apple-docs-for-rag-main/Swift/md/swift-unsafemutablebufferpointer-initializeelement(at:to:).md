

- Swift
- UnsafeMutableBufferPointer
-  initializeElement(at:to:) 

Instance Method

# initializeElement(at:to:)

Initializes the element at `index` to the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func initializeElement(
    at index: UnsafeMutableBufferPointer.Index,
    to value: consuming Element
)
```

## Parameters 

`index`  

The index of the element to initialize

`value`  

The value used to initialize the buffer element’s memory.

## Discussion

The memory underlying the destination element must be uninitialized, or `Element` must be a trivial type. After a call to `initialize(to:)`, the memory underlying this element of the buffer is initialized.

