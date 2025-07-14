

- RealityKit
- FromToByAction
-  init(from:) 

Initializer

# init(from:)

Creates a new instance from a decoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Value` conforms to `AnimatableData`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

Throws an error if reading from `decoder` fails, or if the data is corrupted or otherwise invalid.

