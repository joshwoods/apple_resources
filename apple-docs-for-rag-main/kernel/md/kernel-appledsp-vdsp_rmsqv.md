

- Kernel
- AppleDSP
-  vDSP_rmsqv 

Function

# vDSP_rmsqv

Calculates the root mean square of a single-precision vector.

macOS 10.4+

``` source
void vDSP_rmsqv(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__I`  

The stride for input vector `A`.

`__C`  

The single-precision output scalar.

`__N`  

The number of elements to process. If `N` is zero (`0`), this function returns `NAN`.

## Discussion

This function calculates the root mean square of the first `N` elements of `A` and writes the result to `C`:

The operation is:

C = sqrt(sum(A[n] ** 2, 0 &lt;= n &lt; N) / N);

The following code shows an example of using vDSP_rmsqv:

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var c: Float = .nan

vDSP_rmsqv(a,
           stride,
           &amp;c,
           n)

print(String(format: &quot;RMS %.4f&quot;, c)) // Prints &quot;RMS 2.5434&quot;.

## See Also

### Vector Reduction Functions

vDSP_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

vDSP_svs

Calculates the sum of signed squares in a single-precision vector.

