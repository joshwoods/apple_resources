

- MapKit JS
- mapkit.Annotation
-  callout 

Instance Property

# callout

A delegate that enables you to customize the annotation’s callout.

MapKit JS 5.0+

``` source
attribute AnnotationCalloutDelegate callout;
```

## Discussion

The callout delegate is an optional object that implements methods for customizing the appearance, content, and animations of the callout that appear when selecting the annotation.

See AnnotationCalloutDelegate for details.

## See Also

### Managing callouts

calloutEnabled

A Boolean value that determines whether the map shows an annotation’s callout.

calloutOffset

An offset that changes the annotation callout’s default placement.

