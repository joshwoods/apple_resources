

- MapKit
- MKAnnotationView
-  prepareForDisplay() 

Instance Method

# prepareForDisplay()

Notifies the annotation view that the map view is about to display it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func prepareForDisplay()
```

## Discussion

Use this method to prepare the content of your annotation view.

## See Also

### Creating and preparing an annotation view

init(annotation: (any MKAnnotation)?, reuseIdentifier: String?)

Creates and returns a new annotation view.

init?(coder: NSCoder)

Creates an annotation view using data from the specified unarchiver.

func prepareForReuse()

Calls this method when removing the view from the reuse queue.

