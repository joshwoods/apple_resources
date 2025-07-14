

- MapKit JS
- AnnotationCalloutDelegate
-  calloutAppearanceAnimationForAnnotation 

Instance Method

# calloutAppearanceAnimationForAnnotation

Returns a CSS animation to use when the callout appears.

MapKit JS 5.0+

``` source
string calloutAppearanceAnimationForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

This method returns a string that describes the CSS animation to use for the callout appearance, just like the appearanceAnimation property of mapkit.Annotation.

## Discussion

To animate a callout, MapKit JS calls this method on the annotation’s callout delegate with the annotation as a parameter. A standard callout (with or without custom content) uses a default animation if the callout doesn’t provide the appearance animation.

A callout that uses a custom element can animate only if it provides the appearance animation. The default animation doesn’t apply to callouts with custom elements.

## See Also

### Customizing callout appearance

calloutAnchorOffsetForAnnotation

Returns a point determining the callout’s anchor offset.

calloutShouldAppearForAnnotation

Determines whether the callout appears for an annotation.

calloutShouldAnimateForAnnotation

Determines whether the callout animates.

