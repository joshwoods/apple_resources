

- Metal Performance Shaders Graph
- MPSGraphExecutableExecutionDescriptor
-  signal(\_:atExecutionEvent:value:) 

Instance Method

# signal(\_:atExecutionEvent:value:)

Signals these shared events at execution stage and immediately proceeds.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func signal(
    _ event: any MTLSharedEvent,
    atExecutionEvent executionStage: MPSGraphExecutionStage,
    value: UInt64
)
```

## Parameters 

`event`  

Shared event to signal.

`executionStage`  

Execution stage to signal event at.

`value`  

Value for shared event to wait on.

