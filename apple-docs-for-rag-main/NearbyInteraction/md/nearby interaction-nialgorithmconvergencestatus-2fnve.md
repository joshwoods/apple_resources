

- Nearby Interaction
-  NIAlgorithmConvergenceStatus 

Enumeration

# NIAlgorithmConvergenceStatus

The possible states of Camera Assistance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+watchOS 9.0+

``` source
enum NIAlgorithmConvergenceStatus
```

## Overview

When the app enables Camera Assistance by setting isCameraAssistanceEnabled to `true`, the framework provides the app one of these values in the status field of the convergence object provided by the session(_:didUpdateAlgorithmConvergence:for:) callback.

The framework may require user action before Camera Assistance is fully operational at runtime. This enumeration indicates whether Camera Assistance currently functions as expected on device (convergence state NIAlgorithmConvergenceStatus.converged), and otherwise, the NIAlgorithmConvergenceStatus.Reason defines the recommended user actions when status is NIAlgorithmConvergenceStatus.notConverged(_:).

Note

The Objective-C version of this enumeration is Algorithm Convergence Status.

## Topics

### Interpreting the convergence state

case converged

A status that indicates the framework’s Camera Assistance feature is operational.

case notConverged([NIAlgorithmConvergenceStatus.Reason])

A status that indicates the framework’s Camera Assistance feature requires action from the user.

case unknown

An indication that the framework is unsure of the Camera Assistance status.

### Comparing convergence states

static func == (NIAlgorithmConvergenceStatus, NIAlgorithmConvergenceStatus) -> Bool

Determines whether two convergence statuses are equal.

### Inspecting the convergence state reason

struct Reason

The possible reasons for the Camera Assistance status.

NIAlgorithmConvergenceStatusConverged

A status that indicates the framework’s Camera Assistance feature is operational.

NIAlgorithmConvergenceStatusNotConverged

A status that indicates the framework’s Camera Assistance feature requires action from the user.

NIAlgorithmConvergenceStatusUnknown

An indication that the framework is unsure of the Camera Assistance status.

## Relationships

### Conforms To

- Equatable

## See Also

### Camera assistance

Finding devices with precision

Leverage the spatial awareness of ARKit and Apple Ultra Wideband Chips in your app to guide users to a nearby device.

class NIAlgorithmConvergence

An object that provides the state and reason for user coaching recommendations.

Algorithm Convergence Status

The possible Objective-C states of Camera Assistance.

