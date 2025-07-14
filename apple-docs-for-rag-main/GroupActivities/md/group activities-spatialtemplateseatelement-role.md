

- Group Activities
- SpatialTemplateSeatElement
-  role 

Instance Property

# role

An optional role you associate with this element.

visionOS 2.0+

``` source
let role: (any SpatialTemplateRole)?
```

## Discussion

If you associate a role to a seat, a participant must request that role to sit in the seat. If your template contains seats with roles, include some seats without roles to handle people who are unable to acquire a seat with a role. For example, you might include seats for spectators as well as players of a game.

## See Also

### Getting the element details

let position: SpatialTemplateElementPosition

The location of the element in the shared coordinate space.

let direction: SpatialTemplateElementDirection

The initial orientation of the element in the shared coordinate space.

