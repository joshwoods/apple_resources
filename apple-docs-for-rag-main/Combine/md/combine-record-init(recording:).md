

- Combine
- Record
-  init(recording:) 

Initializer

# init(recording:)

Creates a record publisher from an existing recording.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(recording: Record.Recording)
```

## Parameters 

`recording`  

A previously-recorded recording of published elements and a completion.

## See Also

### Creating a Record Publisher

init(output: [Output], completion: Subscribers.Completion&lt;Failure>)

Creates a record publisher to publish the provided elements, followed by the provided completion value.

init(record: (inout Record&lt;Output, Failure>.Recording) -> Void)

Creates a publisher to interactively record a series of outputs and a completion.

