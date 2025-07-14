

- Group Activities
- SpatialTemplateSeatElement
-  direction 

Instance Property

# direction

The initial orientation of the element in the shared coordinate space.

visionOS 2.0+

``` source
let direction: SpatialTemplateElementDirection
```

## Discussion

The direction you specify rotates the participant’s spatial Persona around the y-axis. This direction becomes the starting point for any further movements the person makes.

## See Also

### Getting the element details

let position: SpatialTemplateElementPosition

The location of the element in the shared coordinate space.

let role: (any SpatialTemplateRole)?

An optional role you associate with this element.

