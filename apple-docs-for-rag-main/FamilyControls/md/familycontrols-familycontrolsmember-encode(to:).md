

- FamilyControls
- FamilyControlsMember
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder, when the type’s `RawValue` is `Int`.

FamilyControlsSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Self` conforms to `Encodable` and `RawValue` is `Int`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

