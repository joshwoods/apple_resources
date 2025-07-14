

- Kernel
- Kernel Functions
-  vDSP_sve_svesq 

Function

# vDSP_sve_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

macOS 10.8+

``` source
void vDSP_sve_svesq(const float *__A, vDSP_Stride __IA, float *__Sum, float *__SumOfSquares, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision input vector.

`__IA`  

Stride for the input vector.

`__Sum`  

Single-precision sum (scalar) of the elements of `A`.

`__SumOfSquares`  

Single-precision sum (scalar) of the squares of the elements of `A`.

`__N`  

Number of elements in `A`.

## Discussion

This function calculates the sum of values and the sum of squares of the first `N` elements of `A` and writes the result to `Sum` and `SumOfSquares` respectively:

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

// Prints &quot;sum 0.1500 sum of squares 38.8125&quot;
print(String(format: &quot;sum %.4f&quot;, sum),
      String(format: &quot;sum of squares %.4f&quot;, sumOfSquares))

