

- Group Activities
- SpatialTemplateSeatElement
-  init(position:direction:role:) 

Initializer

# init(position:direction:role:)

Creates a seat element with the specified position, direction, and role information.

visionOS 2.0+

``` source
init(
    position: SpatialTemplateElementPosition,
    direction: SpatialTemplateElementDirection = .lookingAt(.app),
    role: (any SpatialTemplateRole)? = nil
)
```

## Parameters 

`position`  

The position of this seat in the shared coordinate space. Place seats relative to your app’s content, which is at the origin of the coordinate space.

`direction`  

The initial direction for the participant to face. Specify a value to point the person in the direction of another participant or a specific location in the coordinate space. If you don’t specify this parameter, the participant faces the app’s content.

`role`  

The custom role you assign to the seat. Roles are an optional way to place spatial Personas in an immersive space. For example, you might define roles for two opposing teams in a game and use those roles to place the participants relative to the game content.

## Return Value

An initialized seat element for you to add to a custom spatial template.

