

- Kernel
- Kernel Functions
-  vDSP_vclr 

Function

# vDSP_vclr

Populates a single-precision vector with zeros.

macOS 10.4+

``` source
void vDSP_vclr(float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__C`  

Single-precision real output vector.

`__IC`  

Address stride for `C`.

`__N`  

The number of elements to process.

## Discussion

The vDSP_vclr and vDSP_vclrD functions populate a vector with zeros.

The following code shows how to clear the array c, setting the value of each element to zero:

let n = vDSP_Length(10)
let stride = vDSP_Stride(1)

var c = [Float](repeating: .nan,
                count: Int(n))

vDSP_vclr(&amp;c,
          stride,
          n)

// Prints &quot;[0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]&quot;
print(c)

