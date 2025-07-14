

- MapKit JS
- AnnotationCalloutDelegate
-  calloutContentForAnnotation 

Instance Method

# calloutContentForAnnotation

Returns custom content for the callout bubble.

MapKit JS 5.0+

``` source
Element calloutContentForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

The method returns a DOM element, MapKit JS adds as a subelement of the callout bubble.

## Discussion

You can use this method to provide custom content inside the callout bubble without replacing the whole element, as in calloutElementForAnnotation.

When MapKit JS creates a callout for a selected annotation and the annotation’s callout delegate has no calloutElementForAnnotation method, the framework calls calloutContentForAnnotation method instead — if it’s defined — on the delegate with the annotation as a parameter.

## See Also

### Providing elements

calloutElementForAnnotation

Returns an element representing a custom callout.

calloutLeftAccessoryForAnnotation

Returns an element to use as a custom accessory on the left side of the callout content area.

calloutRightAccessoryForAnnotation

Returns an element to use as a custom accessory on the right side of the callout content area.

