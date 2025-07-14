

- ManagedAppDistribution
- ManagedAppDistributionError
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

