

- MapKit JS
- AnnotationCalloutDelegate
-  calloutElementForAnnotation 

Instance Method

# calloutElementForAnnotation

Returns an element representing a custom callout.

MapKit JS 5.0+

``` source
Element calloutElementForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

This method returns a DOM element to use as the callout element in place of the standard callout bubble. This callout element populates with the information to display, including the information from the annotation.

## Discussion

If you don’t prevent the callout from appearing, MapKit JS calls this method on the annotation’s callout delegate (if the delegate is an object and its calloutElementForAnnotation property is a function) with the annotation as a parameter.

## See Also

### Providing elements

calloutContentForAnnotation

Returns custom content for the callout bubble.

calloutLeftAccessoryForAnnotation

Returns an element to use as a custom accessory on the left side of the callout content area.

calloutRightAccessoryForAnnotation

Returns an element to use as a custom accessory on the right side of the callout content area.

