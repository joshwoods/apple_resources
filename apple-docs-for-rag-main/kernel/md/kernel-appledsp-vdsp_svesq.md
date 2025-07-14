

- Kernel
- AppleDSP
-  vDSP_svesq 

Function

# vDSP_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

macOS 10.4+

``` source
void vDSP_svesq(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__IA`  

The stride for input vector `A`.

`__Sum`  

On return, the single-precision scalar sum of the elements of `A`.

`__SumOfSquares`  

On return, the single-precision scalar sum of the squares of the elements of `A`.

`__N`  

Number of elements in `A`.

## Discussion

This function calculates the sum of values of the first `N` elements of `A` and writes the result to `Sum`. It also calculates the sum of squares of the first `N` elements of `A` and writes the sum to `SumOfSquares`.

The operation is:

Sum          = sum(A[n],      0 &lt;= n &lt; N);
SumOfSquares = sum(A[n] ** 2, 0 &lt;= n &lt; N);

The following code shows an example of using vDSP_sve_svesq:

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var sum: Float = .nan
var sumOfSquares: Float = .nan

vDSP_sve_svesq(a,
               stride,
               &amp;sum,
               &amp;sumOfSquares,
               n)

// Prints &quot;sum 0.1500 sum of squares 38.8125&quot;.
print(String(format: &quot;sum %.4f&quot;, sum),
      String(format: &quot;sum of squares %.4f&quot;, sumOfSquares))

## See Also

### Vector Reduction Functions

vDSP_rmsqv

Calculates the root mean square of a single-precision vector.

vDSP_svs

Calculates the sum of signed squares in a single-precision vector.

