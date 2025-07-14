

- os
- OSSignpostIntervalState
-  encode(to:) 

Instance Method

# encode(to:)

Encodes the interval state into the provided encoder.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func encode(to encoder: any Encoder) throws
```

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

Important

You don’t call this method directly. Instead, the object you’re using to encode the interval state, which must adopt the Encoder protocol, calls it on your behalf as part of the serialization process.

The method throws an error if the interval state is invalid for the specified encoder’s format.

