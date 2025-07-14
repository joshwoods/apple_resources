

- Create ML Components
- NormalizationScaler
-  init(norm:) 

Initializer

# init(norm:)

Creates a normalization scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(norm: NormalizationScaler.NormalizationStrategy = .l2)
```

## Parameters 

`norm`  

A selected NormalizationStrategy to scale by. Defaults as `l2`.

## See Also

### Creating a scaler

enum NormalizationStrategy

A normalization strategy.

