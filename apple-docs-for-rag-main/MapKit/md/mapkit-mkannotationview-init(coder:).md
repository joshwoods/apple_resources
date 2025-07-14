

- MapKit
- MKAnnotationView
-  init(coder:) 

Initializer

# init(coder:)

Creates an annotation view using data from the specified unarchiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The unarchiver to read data from.

## See Also

### Creating and preparing an annotation view

init(annotation: (any MKAnnotation)?, reuseIdentifier: String?)

Creates and returns a new annotation view.

func prepareForReuse()

Calls this method when removing the view from the reuse queue.

func prepareForDisplay()

Notifies the annotation view that the map view is about to display it.

