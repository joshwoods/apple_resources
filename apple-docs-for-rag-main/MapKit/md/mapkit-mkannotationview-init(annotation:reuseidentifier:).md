

- MapKit
- MKAnnotationView
-  init(annotation:reuseIdentifier:) 

Initializer

# init(annotation:reuseIdentifier:)

Creates and returns a new annotation view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
init(
    annotation: (any MKAnnotation)?,
    reuseIdentifier: String?
)
```

## Parameters 

`annotation`  

The annotation object to associate with the new view.

`reuseIdentifier`  

If you plan to reuse the annotation view for similar types of annotations, pass a string to identify it. Although you can pass `nil` if you don’t intend to reuse the view, reusing annotation views is generally best practice.

## Return Value

The initialized annotation view, or `nil` if there’s a problem initializing the object.

## Discussion

The reuse identifier provides a way for you to improve performance by recycling annotation views as the map scrolls on and off of the map. As MapKit no longer needs views, the map view moves them to a reuse queue. When a new annotation becomes visible, your app can request a view for that annotation by passing the appropriate reuse identifier string to the dequeueReusableAnnotationView(withIdentifier:) method of MKMapView.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating and preparing an annotation view

init?(coder: NSCoder)

Creates an annotation view using data from the specified unarchiver.

func prepareForReuse()

Calls this method when removing the view from the reuse queue.

func prepareForDisplay()

Notifies the annotation view that the map view is about to display it.

