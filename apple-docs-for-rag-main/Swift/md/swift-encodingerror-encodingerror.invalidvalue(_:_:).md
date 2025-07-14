

- Swift
- EncodingError
-  EncodingError.invalidValue(\_:\_:) 

Case

# EncodingError.invalidValue(\_:\_:)

An indication that an encoder or its containers could not encode the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case invalidValue(Any, EncodingError.Context)
```

## Discussion

As associated values, this case contains the attempted value and context for debugging.

