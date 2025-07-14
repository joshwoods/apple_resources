

- Kernel
- AppleDSP
-  vDSP_svs 

Function

# vDSP_svs

Calculates the sum of signed squares in a single-precision vector.

macOS 10.4+

``` source
void vDSP_svs(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__I`  

The stride for input vector `A`.

`__C`  

The single-precision output scalar.

`__N`  

The number of elements to process.

## Discussion

This function calculates the mean of the signed squares of the first `N` elements of `A` and writes the result to `C`:

The operation is:

C[0] = sum(A[n] * |A[n]|, 0 &lt;= n &lt; N);

The following code shows an example of using vDSP_svs:

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var c: Float = .nan

vDSP_svs(a,
         stride,
         &amp;c,
         n)

// Prints &quot;sum of signed squares -2.6875&quot;.
print(String(format: &quot;sum of signed squares %.4f&quot;, c))

## See Also

### Vector Reduction Functions

vDSP_rmsqv

Calculates the root mean square of a single-precision vector.

vDSP_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

