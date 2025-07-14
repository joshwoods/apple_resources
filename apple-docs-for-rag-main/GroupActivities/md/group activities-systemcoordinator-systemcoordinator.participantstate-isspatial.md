

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantState
-  isSpatial 

Instance Property

# isSpatial

A Boolean value that indicates whether the person supports being in a shared simulation space for an activity.

visionOS 1.0+

``` source
let isSpatial: Bool
```

## Mentioned in 

Adding spatial Persona support to an activity

## Discussion

The value of this property is `true` when the current person supports activities that place participants relative to the activity itself. The person must use a device that supports spatial experiences, and must configure their spatial Persona to support inclusion in a shared simulation space.

