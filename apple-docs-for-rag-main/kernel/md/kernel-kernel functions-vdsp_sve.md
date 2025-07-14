

- Kernel
- Kernel Functions
-  vDSP_sve 

Function

# vDSP_sve

Calculates the sum of values in a single-precision vector.

macOS 10.4+

``` source
void vDSP_sve(const float *__A, vDSP_Stride __I, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision real input vector.

`__I`  

Stride for `A`.

`__C`  

Single-precision real output scalar.

`__N`  

The number of elements to process.

## Discussion

This function calculates the sum of the first `N` elements of `A` and writes the result to `C`:

The operation is:

C[0] = sum(A[n], 0 &lt;= n &lt; N);

The following code shows an example of using `vDSP_sve`:

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var c: Float = .nan

vDSP_sve(a,
         stride,
         &amp;c,
         n)

// Prints &quot;sum 0.1500&quot;
print(String(format: &quot;sum %.4f&quot;, c))

