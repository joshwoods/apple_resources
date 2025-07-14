

- Group Activities
- SpatialTemplate
-  elements 

Instance Property

# elements

The collection of spatial Persona seats this template contains.

visionOS 2.0+

``` source
var elements: [any SpatialTemplateElement] { get }
```

**Required**

## Discussion

This property contains the seat locations for the participants. Add the seats your template requires, and specify each seat’s location relative to your app’s shared scene. For each seat, you can also specify the direction that seat faces, and optional role information. The system fills seats in the same order they appear in the array.

To place the current participant in a seat with a specific role, use the SystemCoordinator object to assign that role to the participant. The system assigns the first available seat with that role to the participant. If a seat with the requested role is unavailable, the system assigns the participant to the next available seat without a role.

You can specify as many seats as you want in this property, even if there aren’t enough participants to fill all of the seats. If some seats in your template have roles, include enough additional seats without roles to accommodate all participants initially.

