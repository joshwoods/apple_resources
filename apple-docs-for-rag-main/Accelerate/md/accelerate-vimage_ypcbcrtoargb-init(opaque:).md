

- Accelerate
- vImage_YpCbCrToARGB
-  init(opaque:) 

Initializer

# init(opaque:)

Creates a new description of the conversion from YpCbCr to ARGB from the specfied bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(opaque: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))
```

## Parameters 

`opaque`  

The bytes of the opaque representation.

## Discussion

You don’t directly instantiate a vImage_YpCbCrToARGB struct; use vImageConvert_YpCbCrToARGB_GenerateConversion(_:_:_:_:_:_:) to generate a conversion matrix.

## See Also

### Initializers

init()

Creates a new description of the conversion from YpCbCr to ARGB.

