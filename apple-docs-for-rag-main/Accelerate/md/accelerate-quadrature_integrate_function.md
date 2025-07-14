

- Accelerate
-  quadrature_integrate_function 

Structure

# quadrature_integrate_function

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct quadrature_integrate_function
```

## Overview

Describes a real function Y=F(X). Since most of the integration time is spent evaluating F, we allow the caller to provide a array callback, computing several values of F in a single call.

## Topics

### Initializers

init(fun: quadrature_function_array, fun_arg: UnsafeMutableRawPointer!)

### Instance Properties

var fun: quadrature_function_array

var fun_arg: UnsafeMutableRawPointer!

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Type Aliases

typealias quadrature_function_array

struct quadrature_integrate_options

