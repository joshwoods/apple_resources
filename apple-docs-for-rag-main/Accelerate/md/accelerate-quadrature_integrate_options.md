

- Accelerate
-  quadrature_integrate_options 

Structure

# quadrature_integrate_options

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct quadrature_integrate_options
```

## Overview

Can be 0, 15, 21, 31, 41, 51, 61. 0 maps to the default 21. Used by the QAG integrator only. Other integrators ignore this value.

If a workspace is provided, this value is ignored, and the number of intervals is limited by workspace_size. The QNG integrator doesn’t require a workspace. The QAG integrator requires at least max_intervals \* QUADRATURE_INTEGRATE_QAG_WORKSPACE_PER_INTERVAL bytes in workspace. The QAGS integrator requires at least max_intervals \* QUADRATURE_INTEGRATE_QAGS_WORKSPACE_PER_INTERVAL bytes in workspace.

## Topics

### Initializers

init()

init(integrator: quadrature_integrator, abs_tolerance: Double, rel_tolerance: Double, qag_points_per_interval: Int, max_intervals: Int)

### Instance Properties

var abs_tolerance: Double

var integrator: quadrature_integrator

var max_intervals: Int

var qag_points_per_interval: Int

var rel_tolerance: Double

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Type Aliases

typealias quadrature_function_array

struct quadrature_integrate_function

