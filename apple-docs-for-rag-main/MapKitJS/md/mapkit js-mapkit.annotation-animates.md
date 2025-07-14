

- MapKit JS
- mapkit.Annotation
-  animates 

Instance Property

# animates

A Boolean value that determines whether the framework animates the annotation.

MapKit JS 5.0+

``` source
attribute boolean animates;
```

## Discussion

When this property is `true`, MapKit JS animates the appearance of the annotation on the map. You’re responsible for implementing an animation using the appearanceAnimation property.

The annotation doesn’t animate when:

- You don’t provide an animation in appearanceAnimation.

- The animates property is `false.`

## See Also

### Getting and setting interaction behavior

draggable

A Boolean value that determines whether the user can drag the annotation.

selected

A Boolean value that indicates whether the map shows the annotation in a selected state.

enabled

A Boolean value that determines whether the annotation responds to user interaction.

