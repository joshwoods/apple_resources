

- Kernel
- AppleDSP
-  vDSP_vabs 

Function

# vDSP_vabs

Calculates the absolute value of each element in the supplied single-precision vector using the specified stride.

macOS 10.4+

``` source
void vDSP_vabs(const float *__A, vDSP_Stride __IA, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

The single-precision real input vector.

`__IA`  

The stride for input vector `A`.

`__C`  

The single-precision real output vector.

`__IC`  

The stride for output vector `C`.

`__N`  

The number of elements to process.

## Discussion

This function performs the following operation to write the absolute values of the input elements to the corresponding output elements:

