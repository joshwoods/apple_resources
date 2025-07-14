

- Nearby Interaction
- NIAlgorithmConvergenceStatus
- NIAlgorithmConvergenceStatus.Reason
-  insufficientSignalStrength 

Type Property

# insufficientSignalStrength

Indicates that the users might be too far apart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
static let insufficientSignalStrength: NIAlgorithmConvergenceStatus.Reason
```

## Discussion

Coach the user to resolve the issue, such as by presenting text that instructs the user to move closer to the nearby peer or object.

## See Also

### Interpreting the convergence status reason

static let insufficientMovement: NIAlgorithmConvergenceStatus.Reason

Indicates that the device needs to move from its current position in the physical environment.

static let insufficientHorizontalSweep: NIAlgorithmConvergenceStatus.Reason

Indicates that the device needs more horizontal motion.

static let insufficientVerticalSweep: NIAlgorithmConvergenceStatus.Reason

Indicates that the device needs more vertical motion.

static let insufficientLighting: NIAlgorithmConvergenceStatus.Reason

Indicates that the camera needs to view the physical environment under better lighting conditions.

