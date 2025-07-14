

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantState
-  role 

Instance Property

# role

The role assigned to this participant, if any.

visionOS 2.0+

``` source
let role: (any SpatialTemplateRole)?
```

## Discussion

This value could differ from the role attached to the participant’s assigned seat if this participant was assigned a role that has no remaining seats.

