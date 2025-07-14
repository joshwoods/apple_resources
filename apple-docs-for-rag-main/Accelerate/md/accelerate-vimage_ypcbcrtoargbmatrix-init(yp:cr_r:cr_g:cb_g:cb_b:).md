

- Accelerate
- vImage_YpCbCrToARGBMatrix
-  init(Yp:Cr_R:Cr_G:Cb_G:Cb_B:) 

Initializer

# init(Yp:Cr_R:Cr_G:Cb_G:Cb_B:)

Creates a 3 x 3 matrix for converting Y’CbCr signals to RGB.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    Yp: Float,
    Cr_R: Float,
    Cr_G: Float,
    Cb_G: Float,
    Cb_B: Float
)
```

## Parameters 

`Yp`  

The `Yp` in the conversion matrix.

`Cr_R`  

The `Cr_R` in the conversion matrix.

`Cr_G`  

The `Cr_G` in the conversion matrix.

`Cb_G`  

The `Cb_G` in the conversion matrix.

`Cb_B`  

The `Cb_B` in the conversion matrix.

## Return Value

A 3 x 3 matrix for converting Y’CbCr signals to RGB.

## Discussion

The vImage library uses this matrix to convert from YpCbCr to RGB using the following multiplication:

```
                    | R |   | Yp    0     Cr_R |   | Y' |
                    | G | = | Yp   Cb_G   Cr_G | * | Cb |
                    | B |   | Yp   Cb_B     0  |   | Cr |
```

## See Also

### Creating a conversion matrix

init()

Creates a 3 x 3 zero matrix for converting Y’CbCr signals to RGB.

