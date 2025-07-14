

- Metal
- MTLIndirectCommandBufferExecutionRange
-  init(location:length:) 

Initializer

# init(location:length:)

Initializes an command execution range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
init(
    location: UInt32,
    length: UInt32
)
```

## Parameters 

`location`  

The start index of the range.

`length`  

The number of items in the range.

## See Also

### Creating a Command Execution Range

init()

Initializes an empty command execution range.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

