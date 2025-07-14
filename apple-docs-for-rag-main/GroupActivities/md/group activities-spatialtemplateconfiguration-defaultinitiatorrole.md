

- Group Activities
- SpatialTemplateConfiguration
-  defaultInitiatorRole 

Instance Property

# defaultInitiatorRole

The default role to assign to the initiator of the group activity.

visionOS 2.0+

``` source
let defaultInitiatorRole: (any SpatialTemplateRole)?
```

## Discussion

Spatial templates use roles to determine which seats are available to participants. If you specify a value for this property at initialization time, the spatial template assigns this role to the person who starts the group activity. For example, you might assign a presenter role to the person who starts an activity to deliver a presentation.

