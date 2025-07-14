

- WatchKit
- WKGestureRecognizer
-  objectBounds() 

Instance Method

# objectBounds()

Returns the dimensions of the interface object (measured in points) associated with the gesture recognizer.

watchOS 3.0+

``` source
func objectBounds() -> CGRect
```

## Return Value

The bounding rectangle of the interface object to which the gesture recognizer is attached.

## Discussion

You attach a gesture recognizer to a specific element in your storyboard file. At runtime, you use this property to get the dimensions of that element.

## See Also

### Getting the Touch Information

func locationInObject() -> CGPoint

Returns the point computed as the current position of the touch event.

