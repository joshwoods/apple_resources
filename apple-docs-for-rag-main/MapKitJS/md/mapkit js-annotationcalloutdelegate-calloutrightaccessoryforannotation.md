

- MapKit JS
- AnnotationCalloutDelegate
-  calloutRightAccessoryForAnnotation 

Instance Method

# calloutRightAccessoryForAnnotation

Returns an element to use as a custom accessory on the right side of the callout content area.

MapKit JS 5.0+

``` source
Element calloutRightAccessoryForAnnotation(
 mapkit.Annotation annotation
);
```

## Parameters 

`annotation`  

The annotation for the callout.

## Return Value

This method returns a DOM element to display as the right accessory.

## Discussion

You can use this method to provide a custom accessory to the right side of the callout content area. It works similarly to calloutLeftAccessoryForAnnotation.

## See Also

### Providing elements

calloutContentForAnnotation

Returns custom content for the callout bubble.

calloutElementForAnnotation

Returns an element representing a custom callout.

calloutLeftAccessoryForAnnotation

Returns an element to use as a custom accessory on the left side of the callout content area.

