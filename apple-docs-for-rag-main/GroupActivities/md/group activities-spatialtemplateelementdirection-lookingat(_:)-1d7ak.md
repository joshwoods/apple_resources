

- Group Activities
- SpatialTemplateElementDirection
-  lookingAt(\_:) 

Type Method

# lookingAt(\_:)

Creates a direction that orients the participant to face the specified point in the shared coordinate space.

visionOS 2.0+

``` source
static func lookingAt(_ position: SpatialTemplateElementPosition) -> SpatialTemplateElementDirection
```

## Parameters 

`position`  

A location in the shared coordinate space. Specify positions as an offset from the app’s content using the SpatialTemplateElementPosition type.

## Return Value

A direction type that faces the specified position in the coordinate space.

## See Also

### Looking at a specific location

static func lookingAt(any SpatialTemplateElement) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to face another template element.

