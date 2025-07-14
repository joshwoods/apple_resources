

- Kernel
- AppleDSP
-  vDSP_vma 

Function

# vDSP_vma

Adds a single-precision vector to the product of two single-precision vectors.

macOS 10.4+

``` source
void vDSP_vma(const float *__A, vDSP_Stride __IA, const float *__B, vDSP_Stride __IB, const float *__C, vDSP_Stride __IC, float *__D, vDSP_Stride __ID, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector `A`.

`__IA`  

The stride for input vector `A`.

`__B`  

The single-precision real input vector `B`.

`__IB`  

The stride for input vector `B`.

`__C`  

The single-precision real input vector `C`.

`__IC`  

The stride for input vector `C`.

`__D`  

The single-precision real output vector.

`__ID`  

The stride for output vector `D`.

`__N`  

The number of elements to process.

## Discussion

This function calculates the products of the first `N` elements of `A` and `B`, adds each product to the corresponding value in `C`, and writes the result to `D`:

The operation is:

 for (n = 0; n &lt; N; ++n)
    D[n] = A[n] * B[n] + C[n];

The following code shows an example of using vDSP_vma:

let stride = vDSP_Stride(1)

let a: [Float] = [10, 20, 30, 40, 50]
let b: [Float] = [ 1,  2,  3,  4,  5]

let c: [Float] = [1, 2, 3, 4, 5]

let n = vDSP_Length(a.count)

var d = [Float](repeating: 0,
                count: a.count)

vDSP_vma(a, stride,
         b, stride,
         c, stride,
         &amp;d, stride,
         n)

// Prints &quot;[11.0, 42.0, 93.0, 164.0, 255.0]&quot;.
print(d)

## See Also

### Vector Arithmetic Functions

vDSP_vadd

Adds two single-precision vectors.

vDSP_vsub

Subtracts two single-precision vectors.

vDSP_vmul

Multiplies two single-precision vectors.

vDSP_vsmul

Multiplies a single-precision scalar value by a single-precision vector.

vDSP_vdiv

Divides two single-precision vectors.

