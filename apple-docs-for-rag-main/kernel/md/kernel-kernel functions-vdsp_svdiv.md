

- Kernel
- Kernel Functions
-  vDSP_svdiv 

Function

# vDSP_svdiv

Divides a single-precision scalar value by a single-precision vector.

macOS 10.4+

``` source
void vDSP_svdiv(const float *__A, const float *__B, vDSP_Stride __IB, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Pointer to single-precision real input scalar.

`__B`  

Single-precision real input vector.

`__IB`  

Stride for `B`.

`__C`  

Single-precision real output vector.

`__IC`  

Stride for `C`.

`__N`  

The number of elements to process.

## Discussion

This function calculates the scalar value `A` divied by the first `N` elements of `B`, writing the result to `C`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    C[n] = A / B[n];

The following code shows an example of using vDSP_vsdiv:

let stride = vDSP_Stride(1)

var a: Float = 2
let b: [Float] = [1, 2, 4, 5]

let n = vDSP_Length(b.count)

var c = [Float](repeating: 0,
                count: b.count)

vDSP_svdiv(&amp;a,
           b, stride,
           &amp;c, stride,
           n)

// Prints &quot;[2, 1, 0.5, 0.4]&quot;
print(c)

