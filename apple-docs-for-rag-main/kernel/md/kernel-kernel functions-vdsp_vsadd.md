

- Kernel
- Kernel Functions
-  vDSP_vsadd 

Function

# vDSP_vsadd

Adds a single-precision scalar value to a single-precision vector.

macOS 10.4+

``` source
void vDSP_vsadd(const float *__A, vDSP_Stride __IA, const float *__B, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Single-precision real input vector.

`__IA`  

Stride for `A.`

`__B`  

Pointer to single-precision real input scalar.

`__C`  

Single-precision real output vector.

`__IC`  

Stride for `C.`

`__N`  

The number of elements to process.

## Discussion

This function calculates the sums of the first `N` elements of `A` and the scalar value `B`, writing the result to `C`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    C[n] = A[n] + B[0];

The following code shows an example of using vDSP_vsadd:

let a: [Float] = [1, 2, 4, 5]
var b: Float = 2

let n = vDSP_Length(a.count)

var c = [Float](repeating: 0,
                count: a.count)

vDSP_vsadd(a, stride,
           &amp;b,
           &amp;c, stride,
           n)

// Prints &quot;[3.0, 4.0, 6.0, 7.0]&quot;
print(c)

