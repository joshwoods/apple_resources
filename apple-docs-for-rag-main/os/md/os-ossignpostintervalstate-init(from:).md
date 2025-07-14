

- os
- OSSignpostIntervalState
-  init(from:) 

Initializer

# init(from:)

Decodes the interval state from the provided decoder.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
required init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

Important

You don’t call this method directly. Instead, the object you’re using to decode the interval state, which must adopt the Decoder protocol, calls it on your behalf as part of the serialization process.

The initializer throws an error if reading from the decoder fails, or if the decoder’s data is corrupt or invalid.

