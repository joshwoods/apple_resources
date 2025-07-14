

- Group Activities
- SpatialTemplateElementDirection
-  lookingAt(\_:) 

Type Method

# lookingAt(\_:)

Creates a direction that orients the participant to face another template element.

visionOS 2.0+

``` source
static func lookingAt(_ element: any SpatialTemplateElement) -> SpatialTemplateElementDirection
```

## Parameters 

`element`  

The template element to look at.

## Return Value

A direction type that faces the specified seat position.

## Discussion

Call this method when you want one participant to look at another participant.

## See Also

### Looking at a specific location

static func lookingAt(SpatialTemplateElementPosition) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to face the specified point in the shared coordinate space.

