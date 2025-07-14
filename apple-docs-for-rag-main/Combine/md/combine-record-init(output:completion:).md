

- Combine
- Record
-  init(output:completion:) 

Initializer

# init(output:completion:)

Creates a record publisher to publish the provided elements, followed by the provided completion value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    output: [Output],
    completion: Subscribers.Completion
)
```

## Parameters 

`output`  

An array of output elements to publish.

`completion`  

The completion value with which to end publishing.

## See Also

### Creating a Record Publisher

init(record: (inout Record&lt;Output, Failure>.Recording) -> Void)

Creates a publisher to interactively record a series of outputs and a completion.

init(recording: Record&lt;Output, Failure>.Recording)

Creates a record publisher from an existing recording.

