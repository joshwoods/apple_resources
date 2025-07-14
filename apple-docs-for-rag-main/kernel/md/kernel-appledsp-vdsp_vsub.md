

- Kernel
- AppleDSP
-  vDSP_vsub 

Function

# vDSP_vsub

Subtracts two single-precision vectors.

macOS 10.0+

``` source
void vDSP_vsub(const float *__B, vDSP_Stride __IB, const float *__A, vDSP_Stride __IA, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__B`  

The single-precision real input vector `B`.

`__IB`  

The stride for input vector `B`.

`__A`  

The single-precision real input vector `A`.

`__IA`  

The stride for input vector `A`.

`__C`  

The single-precision real output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

Number of elements to subtract.

## Discussion

This function calculates the differences of the first `N` elements of input vectors `A` and `B`, writing the result to output vector `C`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    C[n] = A[n] - B[n];

The following code shows an example of using vDSP_vsub:

let stride = vDSP_Stride(1)

let a: [Float] = [1, 2, 3, 4, 5]
let b: [Float] = [10, 20, 30, 40, 50]

let n = vDSP_Length(a.count)

var c = [Float](repeating: 0,
                count: a.count)

vDSP_vsub(b, stride,
          a, stride,
          &amp;c, stride,
          n)

// Prints &quot;[-9.0, -18.0, -27.0, -36.0, -45.0]&quot;.
print(c)

## See Also

### Vector Arithmetic Functions

vDSP_vadd

Adds two single-precision vectors.

vDSP_vma

Adds a single-precision vector to the product of two single-precision vectors.

vDSP_vmul

Multiplies two single-precision vectors.

vDSP_vsmul

Multiplies a single-precision scalar value by a single-precision vector.

vDSP_vdiv

Divides two single-precision vectors.

