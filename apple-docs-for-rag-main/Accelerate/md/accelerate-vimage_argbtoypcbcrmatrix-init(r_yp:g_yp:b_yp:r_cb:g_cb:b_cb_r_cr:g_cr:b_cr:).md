

- Accelerate
- vImage_ARGBToYpCbCrMatrix
-  init(R_Yp:G_Yp:B_Yp:R_Cb:G_Cb:B_Cb_R_Cr:G_Cr:B_Cr:) 

Initializer

# init(R_Yp:G_Yp:B_Yp:R_Cb:G_Cb:B_Cb_R_Cr:G_Cr:B_Cr:)

Creates a 3 x 3 matrix for converting RGB to Y’CbCr.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    R_Yp: Float,
    G_Yp: Float,
    B_Yp: Float,
    R_Cb: Float,
    G_Cb: Float,
    B_Cb_R_Cr: Float,
    G_Cr: Float,
    B_Cr: Float
)
```

## Parameters 

`R_Yp`  

The *R_Yp* in the conversion matrix.

`G_Yp`  

The *G_Yp* in the conversion matrix.

`B_Yp`  

The *B_Yp* in the conversion matrix.

`R_Cb`  

The *R_Cb* in the conversion matrix.

`G_Cb`  

The *G_Cb* in the conversion matrix.

`B_Cb_R_Cr`  

The *B_Cb_R_Cr* in the conversion matrix.

`G_Cr`  

The *G_Cr* in the conversion matrix.

`B_Cr`  

The *B_Cr* in the conversion matrix.

## Discussion

The 3 x 3 matrix is given by:

## See Also

### Creating a conversion matrix

init()

Creates a 3 x 3 zero matrix for converting RGB to Y’CbCr.

