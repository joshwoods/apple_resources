

- Metal Performance Shaders Graph
- MPSGraphExecutableExecutionDescriptor
-  wait(for:value:) 

Instance Method

# wait(for:value:)

Waits on these shared events before scheduling execution on the HW.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func wait(
    for event: any MTLSharedEvent,
    value: UInt64
)
```

## Parameters 

`event`  

Shared event to wait on.

`value`  

Value for shared event to wait on.

## Discussion

This does not include encoding which can still continue.

