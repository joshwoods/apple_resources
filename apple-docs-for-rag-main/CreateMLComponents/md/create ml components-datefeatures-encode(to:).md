

- Create ML Components
- DateFeatures
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Self` conforms to `Encodable` and `RawValue` is `Int`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

