

- Swift
- UnsafeMutableBufferPointer
-  update(repeating:) 

Instance Method

# update(repeating:)

Updates every element of this buffer’s initialized memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func update(repeating repeatedValue: Element)
```

## Parameters 

`repeatedValue`  

The value used when updating this pointer’s memory.

## Discussion

The buffer’s memory must be initialized or its `Element` type must be a trivial type.

Note

All buffer elements must already be initialized.

