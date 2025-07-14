

- Kernel
- Kernel Functions
-  vDSP_vfill 

Function

# vDSP_vfill

Populates a single-precision vector with a specified scalar value.

macOS 10.4+

``` source
void vDSP_vfill(const float *__A, float *__C, vDSP_Stride __IC, vDSP_Length __N);
```

## Parameters 

`__A`  

Pointer to single-precision real input scalar.

`__C`  

Single-precision real output vector.

`__IC`  

Address stride for `C`.

`__N`  

The number of elements to process.

## Discussion

The functions in this group populate a vector with a specified scalar value.

The following code shows how to clear the array c, setting the value of each element to pi:

let n = vDSP_Length(10)
let stride = vDSP_Stride(1)

var a = Float.pi

var c = [Float](repeating: .nan,
                count: Int(n))

vDSP_vfill(&amp;a,
           &amp;c,
           stride,
           n)

// Prints &quot;[3.1415925, 3.1415925, 3.1415925,
//          3.1415925, 3.1415925, 3.1415925,
//          3.1415925, 3.1415925, 3.1415925,
//          3.1415925]&quot;
print(c)

