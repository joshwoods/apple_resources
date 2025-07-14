

- Swift
- UInt16
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(to encoder: any Encoder) throws
```

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

