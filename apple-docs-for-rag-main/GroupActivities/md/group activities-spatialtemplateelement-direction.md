

- Group Activities
- SpatialTemplateElement
-  direction 

Instance Property

# direction

The initial orientation of the element in the shared coordinate space.

visionOS 2.0+

``` source
var direction: SpatialTemplateElementDirection { get }
```

**Required**

## Discussion

The direction you specify rotates the participant’s spatial Persona around the y-axis. This direction becomes the starting point for any further movements the person makes.

## See Also

### Getting the element details

var position: SpatialTemplateElementPosition

The location of the element in the shared coordinate space.

**Required**

var role: (any SpatialTemplateRole)?

An optional role you associate with this element.

**Required**

