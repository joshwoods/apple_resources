

- Accelerate
- Quadrature
- Quadrature.Integrator
-  Quadrature.Integrator.qag(pointsPerInterval:maxIntervals:) 

Case

# Quadrature.Integrator.qag(pointsPerInterval:maxIntervals:)

Globally adaptive integrator.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case qag(
    pointsPerInterval: Quadrature.QAGPointsPerInterval,
    maxIntervals: Int
)
```

## See Also

### Integrators

case qng

Non-adaptive automatic integrator that uses Gauss-Kronrod-Patterson quadrature coefficients.

static let nonAdaptive: Quadrature.Integrator

Non-adaptive automatic integrator that uses Gauss-Kronrod-Patterson quadrature coefficients.

static func adaptive(pointsPerInterval: Quadrature.QAGPointsPerInterval, maxIntervals: Int) -> Quadrature.Integrator

Globally adaptive integrator.

case qags(maxIntervals: Int)

Globally adaptive integrator that is based on 21-point or 15-point Gauss–Kronrod quadrature within each subinterval.

static func adaptiveWithSingularities(maxIntervals: Int) -> Quadrature.Integrator

Globally adaptive integrator that is based on 21-point or 15-point Gauss–Kronrod quadrature within each subinterval.

