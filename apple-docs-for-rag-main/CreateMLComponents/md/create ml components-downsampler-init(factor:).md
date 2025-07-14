

- Create ML Components
- Downsampler
-  init(factor:) 

Initializer

# init(factor:)

Creates a down sample temporal transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(factor: Int)
```

## Parameters 

`factor`  

The down sample factor to the input stream.

## Discussion

Precondition

`factor` must be greater than 0.

## See Also

### Creating a transformer

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

