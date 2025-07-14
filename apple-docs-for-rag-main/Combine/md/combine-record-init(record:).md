

- Combine
- Record
-  init(record:) 

Initializer

# init(record:)

Creates a publisher to interactively record a series of outputs and a completion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(record: (inout Record.Recording) -> Void)
```

## Parameters 

`record`  

A recording instance that can be retrieved after completion to create new record publishers to replay the recording.

## See Also

### Creating a Record Publisher

init(output: [Output], completion: Subscribers.Completion&lt;Failure>)

Creates a record publisher to publish the provided elements, followed by the provided completion value.

init(recording: Record&lt;Output, Failure>.Recording)

Creates a record publisher from an existing recording.

