

- Kernel
- AppleDSP
-  vDSP_vsmul 

Function

# vDSP_vsmul

Multiplies a single-precision scalar value by a single-precision vector.

macOS 10.0+

``` source
void vDSP_vsmul(const float *__A, vDSP_Stride __IA, const float *__B, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__IA`  

The stride for input vector `A`.

`__B`  

A pointer to the single-precision real input scalar.

`__C`  

The single-precision real output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of elements to multiply.

## Discussion

This function calculates the products of the first `N` elements of `A` and the scalar value `B`, writing the result to `C`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    C[n] = A[n] * B;

The following code shows an example of using vDSP_vsmul:

let stride = vDSP_Stride(1)

let a: [Float] = [1, 2, 4, 5]
var b: Float = 2

let n = vDSP_Length(a.count)

var c = [Float](repeating: 0,
                count: a.count)

vDSP_vsmul(a, stride,
           &amp;b,
           &amp;c, stride,
           n)

// Prints &quot;[2.0, 4.0, 8.0, 10.0]&quot;.
print(c)

## See Also

### Vector Arithmetic Functions

vDSP_vadd

Adds two single-precision vectors.

vDSP_vma

Adds a single-precision vector to the product of two single-precision vectors.

vDSP_vsub

Subtracts two single-precision vectors.

vDSP_vmul

Multiplies two single-precision vectors.

vDSP_vdiv

Divides two single-precision vectors.

