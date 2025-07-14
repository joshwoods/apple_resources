

- MapKit
- MKAnnotationView
-  prepareForReuse() 

Instance Method

# prepareForReuse()

Calls this method when removing the view from the reuse queue.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func prepareForReuse()
```

## Discussion

The default implementation of this method does nothing. You can override it in your custom annotation views and use it to put the view in a known state before the map view returns it to your map view delegate.

## See Also

### Related Documentation

func dequeueReusableAnnotationView(withIdentifier: String) -> MKAnnotationView?

Returns a reusable annotation view using its identifier.

### Creating and preparing an annotation view

init(annotation: (any MKAnnotation)?, reuseIdentifier: String?)

Creates and returns a new annotation view.

init?(coder: NSCoder)

Creates an annotation view using data from the specified unarchiver.

func prepareForDisplay()

Notifies the annotation view that the map view is about to display it.

