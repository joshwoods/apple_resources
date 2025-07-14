

- Create ML Components
- Downsampler
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Down samples the input sequence

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler?
) throws -> Downsampler.DownStreamSequence where Input == S.Feature, S : TemporalSequence
```

## Parameters 

`input`  

An async sequence of inputs.

`eventHandler`  

An event handler.

## Return Value

An async sequence of down sampled outputs.

## See Also

### Performing the transformation

typealias Input

The input type.

typealias Output

The output type.

struct DownStreamSequence

An async sequence of down stream elements.

