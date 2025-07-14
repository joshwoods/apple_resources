

- Accelerate
-  quadrature_function_array 

Type Alias

# quadrature_function_array

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias quadrature_function_array = (UnsafeMutableRawPointer?, Int, UnsafePointer, UnsafeMutablePointer) -> Void
```

## Parameters 

`arg`  

User argument passed back to the function when evaluated

`n`  

Dimension of arrays X and Y

`x`  

Array of points to evaluate the function

`y`  

Array receiving the values

## Discussion

Should set values y\[i\] = F(x\[i\]) for i=0..n-1.

## See Also

### Type Aliases

struct quadrature_integrate_function

struct quadrature_integrate_options

