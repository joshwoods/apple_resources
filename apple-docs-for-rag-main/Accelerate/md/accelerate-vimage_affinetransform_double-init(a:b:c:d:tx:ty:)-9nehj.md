

- Accelerate
- vImage_AffineTransform_Double
-  init(a:b:c:d:tx:ty:) 

Initializer

# init(a:b:c:d:tx:ty:)

Returns a new affine transform.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    a: Double,
    b: Double,
    c: Double,
    d: Double,
    tx: Double,
    ty: Double
)
```

## Parameters 

`a`  

The entry at position `[1,1]` in the matrix.

`b`  

The entry at position `[1,2]` in the matrix.

`c`  

The entry at position `[2,1]` in the matrix.

`d`  

The entry at position `[2,2]` in the matrix.

`tx`  

The entry at position `[3,1]` in the matrix.

`ty`  

The entry at position `[3,2]` in the matrix.

## Discussion

## See Also

### Initializers

init()

init(a: CGFloat, b: CGFloat, c: CGFloat, d: CGFloat, tx: CGFloat, ty: CGFloat)

