

- MapKit JS
- AnnotationCalloutDelegate
-  calloutShouldAppearForAnnotation 

Instance Method

# calloutShouldAppearForAnnotation

Determines whether the callout appears for an annotation.

MapKit JS 5.0+

``` source
boolean calloutShouldAppearForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

The method returns a Boolean value, where a value of `false` prevents the callout from appearing.

## Discussion

When the user selects an annotation, MapKit JS calls this method on the annotation’s callout delegate (if the delegate is an object and its calloutShouldAppearForAnnotation property is a function) with the annotation as a parameter.

## See Also

### Customizing callout appearance

calloutAnchorOffsetForAnnotation

Returns a point determining the callout’s anchor offset.

calloutShouldAnimateForAnnotation

Determines whether the callout animates.

calloutAppearanceAnimationForAnnotation

Returns a CSS animation to use when the callout appears.

