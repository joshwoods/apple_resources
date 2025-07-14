

- Kernel
- AppleDSP
-  vDSP_maxmgv 

Function

# vDSP_maxmgv

Calculates the maximum magnitude in a single-precision vector.

macOS 10.4+

``` source
void vDSP_maxmgv(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__I`  

The stride for input vector `A`.

`__C`  

The single-precsion output scalar.

`__N`  

The number of elements to process. If `N` is zero (`0`), this function returns `-INFINITY`.

## Discussion

This function calculates the maximum magnitude of the first `N` elements of `A` and writes the result to `C`:

The operation is:

*C = -INFINITY;
for (n = 0; n &lt; N; ++n)
    if (*C &lt; |A[n*I]|)
        *C = |A[n*I]|;

The following code shows an example of using vDSP_maxmgv.

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var c: Float = .nan

vDSP_maxmgv(a,
            stride,
            &amp;c,
            n)

print(&quot;max magnitude&quot;, c) // Prints &quot;max magnitude 4.3&quot;.

