

- Foundation
- JSONEncoder
- JSONEncoder.DataEncodingStrategy
-  JSONEncoder.DataEncodingStrategy.custom(\_:) 

Case

# JSONEncoder.DataEncodingStrategy.custom(\_:)

The strategy that encodes data using a user-defined function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
case custom((Data, any Encoder) throws -> Void)
```

## Parameters 

`custom`  

A closure that receives the data to encode and the encoder instance to encode to.

## Discussion

If the user-defined function throws, the encoder uses an empty container in place of the data.

