

- MapKit JS
- AnnotationCalloutDelegate
-  calloutShouldAnimateForAnnotation 

Instance Method

# calloutShouldAnimateForAnnotation

Determines whether the callout animates.

MapKit JS 5.0+

``` source
boolean calloutShouldAnimateForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

This method returns a Boolean value that determines if the callout should be animated.

## Discussion

This method determines whether an appearance annotation should run. The animation runs if the value is `true`.

## See Also

### Customizing callout appearance

calloutAnchorOffsetForAnnotation

Returns a point determining the callout’s anchor offset.

calloutShouldAppearForAnnotation

Determines whether the callout appears for an annotation.

calloutAppearanceAnimationForAnnotation

Returns a CSS animation to use when the callout appears.

