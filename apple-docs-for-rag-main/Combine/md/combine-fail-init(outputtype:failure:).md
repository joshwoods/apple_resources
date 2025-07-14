

- Combine
- Fail
-  init(outputType:failure:) 

Initializer

# init(outputType:failure:)

Creates publisher with the given output type, that immediately terminates with the specified failure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    outputType: Output.Type,
    failure: Failure
)
```

## Parameters 

`outputType`  

The output type exposed by this publisher.

`failure`  

The failure to send when terminating the publisher.

## Discussion

Use this initializer to create a `Fail` publisher that can work with subscribers or publishers that expect a given output type.

## See Also

### Creating a Fail Publisher

init(error: Failure)

Creates a publisher that immediately terminates with the specified failure.

