

- Core ML
- MLFeatureValue
- MLFeatureValue.ImageOption
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates an image feature option key from a raw value string.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

A string that represents the name of the image feature option key.

## Discussion

Don’t use this initializer directly. Create an image option key with cropAndScale or cropRect instead.

## See Also

### Image Option Key Initializers

init(String)

Creates an image feature option key from a string.

