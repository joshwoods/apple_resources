

- MapKit JS
- mapkit.Annotation
-  calloutEnabled 

Instance Property

# calloutEnabled

A Boolean value that determines whether the map shows an annotation’s callout.

MapKit JS 5.0+

``` source
attribute boolean calloutEnabled;
```

## Discussion

If the title is empty, the framework can’t show the standard callout even if this property is `true`.

## See Also

### Managing callouts

callout

A delegate that enables you to customize the annotation’s callout.

calloutOffset

An offset that changes the annotation callout’s default placement.

