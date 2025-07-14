

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantState
-  seat 

Instance Property

# seat

The seat assigned to this participant.

visionOS 2.0+

``` source
let seat: SystemCoordinator.ParticipantState.Seat?
```

## Discussion

If this value is `nil`, either the participant is non-spatial or there is no seat available for the participant.

