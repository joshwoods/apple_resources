

- Combine
- Fail
-  init(error:) 

Initializer

# init(error:)

Creates a publisher that immediately terminates with the specified failure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(error: Failure)
```

## Parameters 

`error`  

The failure to send when terminating the publisher.

## See Also

### Creating a Fail Publisher

init(outputType: Output.Type, failure: Failure)

Creates publisher with the given output type, that immediately terminates with the specified failure.

