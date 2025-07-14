

- MapKit JS
- AnnotationConstructorOptions
-  calloutOffset 

Instance Property

# calloutOffset

The offset, in CSS pixels, of a callout from the top center of the element.

MapKit JS 5.0+

``` source
attribute DOMPoint calloutOffset;
```

## Discussion

The default value is `DOMPoint(0, 1)`, placing the callout bubble is slightly (1 pixel) above the top-center point of the annotation element.

To choose a different placement, provide an offset point where positive x values move the callout bubble to the left, and positive y values move the callout bubble up. For example, to leave a 5px margin between the top of the annotation and the bottom of the callout, use a callout offset of `DOMPoint(0, 5)`.

## See Also

### Creating callouts

callout

A delegate that enables you to customize the annotation’s callout.

calloutEnabled

A Boolean value that determines whether the map shows a callout.

