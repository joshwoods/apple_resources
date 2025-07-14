

- Accelerate
-  Quadrature 

Structure

# Quadrature

A structure that approximates the definite integral of a function over a finite interval.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct Quadrature
```

## Overview

The following code illustrates using a Quadrature structure to calculate the area under a curve, defined by `y = sqrt(radius * radius - pow(x - radius, 2))`:

```
let quadrature = Quadrature(integrator: .qags(maxIntervals: 10),
                            absoluteTolerance: 1.0e-8,
                            relativeTolerance: 1.0e-2)

let result = quadrature.integrate(over: 0.0 ... 25.0) { x in
    let radius: Double = 12.5
    return sqrt(radius * radius - pow(x - radius, 2))
}

switch result {
case .success(let integralResult, let estimatedAbsoluteError):
    print("quadrature success:", integralResult,
          estimatedAbsoluteError)
case .failure(let error):
    print("quadrature error:", error.errorDescription)
}
```

Alternatively, you can integrate over a function that uses vectors for its source and destination. For example:

```
func vectorExp(x: UnsafeBufferPointer,
               y: UnsafeMutableBufferPointer) {
    let radius: Double = 12.5
    for i in 0 ..

## Topics

### Initializers

init(integrator: Quadrature.Integrator, absoluteTolerance: Double, relativeTolerance: Double)

Initializes and returns a quadrature instance.

### Instance Properties

var absoluteTolerance: Double

The requested absolute tolerance on the result.

var relativeTolerance: Double

The requested relative tolerance on the result.

### Instance Methods

func integrate(over: ClosedRange&lt;Double>, integrand: (Double) -> Double) -> Result&lt;(integralResult: Double, estimatedAbsoluteError: Double), Quadrature.Error>

Performs the integration over the supplied scalar function.

func integrate(over: ClosedRange&lt;Double>, integrand: (UnsafeBufferPointer&lt;Double>, UnsafeMutableBufferPointer&lt;Double>) -> ()) -> Result&lt;(integralResult: Double, estimatedAbsoluteError: Double), Quadrature.Error>

Performs the integration over the supplied vector function.

### Structures

struct QAGPointsPerInterval

Constants that specify the number of points per interval for the globally adaptive integrator.

### Enumerations

enum Error

Errors thrown by the Quadrature structure.

enum Integrator

Constants that define different integrators.

### Type Aliases

typealias quadrature_function_array

struct quadrature_integrate_function

struct quadrature_integrate_options

## See Also

### Quadrature

struct quadrature_integrator

Constants that specify integration algorithms.

struct quadrature_status

Constants that indicate the status of a quadrature operation.

