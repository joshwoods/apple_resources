

- WatchKit
- WKPanGestureRecognizer
-  translationInObject() 

Instance Method

# translationInObject()

The amount of translation for the pan gesture in the current object.

watchOS 3.0+

``` source
func translationInObject() -> CGPoint
```

## Return Value

A point representing the translation value relative to the current object’s coordinate system.

## Discussion

The x and y values report the total translation over time. They are not delta values from the last time that the translation was reported.

## See Also

### Tracking the Location and Velocity of the Gesture

func velocityInObject() -> CGPoint

The velocity of the pan gesture in the current object.

