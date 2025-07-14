

- Combine
- Empty
-  init(completeImmediately:outputType:failureType:) 

Initializer

# init(completeImmediately:outputType:failureType:)

Creates an empty publisher with the given completion behavior and output and failure types.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    completeImmediately: Bool = true,
    outputType: Output.Type,
    failureType: Failure.Type
)
```

## Parameters 

`completeImmediately`  

A Boolean value that indicates whether the publisher should immediately finish.

`outputType`  

The output type exposed by this publisher.

`failureType`  

The failure type exposed by this publisher.

## Discussion

Use this initializer to connect the empty publisher to subscribers or other publishers that have specific output and failure types.

## See Also

### Creating an Empty Publisher

init(completeImmediately: Bool)

Creates an empty publisher.

