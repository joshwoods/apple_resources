

- MapKit
- MKOverlayPathRenderer
-  createPath() 

Instance Method

# createPath()

Creates the path for the overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func createPath()
```

## Discussion

The default implementation of this method does nothing. Subclasses can override it and use it to create the CGPath data type the subclass uses for drawing. After creating the path, your implementation needs to assign it to the path property.

## See Also

### Creating and managing the path

var path: CGPath!

The path representing the overlay’s shape.

func invalidatePath()

Updates the path associated with the overlay renderer.

