

- Kernel
- Kernel Functions
-  vDSP_minv 

Function

# vDSP_minv

Calculates the minimum value in a single-precision vector.

macOS 10.4+

``` source
void vDSP_minv(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision real input vector.

`__I`  

Stride for `A.`

`__C`  

Output scalar.

`__N`  

The number of elements to process. If `N` is zero (`0`), this function returns `-INFINITY`.

## Discussion

This function calculates the minimum value of the first `N` elements of `A `and writes the result to `C`:

The operation is:

*C = +INFINITY;
for (n = 0; n &lt; N; ++n)
    if (*C > A[n*I])
        *C = A[n*I];

The following code shows an example of using vDSP_minv.

let stride = vDSP_Stride(1)

let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]
let n = vDSP_Length(a.count)

var c: Float = .nan

vDSP_minv(a,
          stride,
          &amp;c,
          n)

print(&quot;min&quot;, c) // Prints &quot;min -4.3&quot;

