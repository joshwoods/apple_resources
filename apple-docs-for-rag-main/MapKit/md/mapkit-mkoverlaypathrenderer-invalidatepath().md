

- MapKit
- MKOverlayPathRenderer
-  invalidatePath() 

Instance Method

# invalidatePath()

Updates the path associated with the overlay renderer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func invalidatePath()
```

## Discussion

Call this method when a change in the path information would require you to recreate the overlay’s path. This method sets the path property to `nil` and tells the overlay renderer to redisplay its contents.

## See Also

### Creating and managing the path

var path: CGPath!

The path representing the overlay’s shape.

func createPath()

Creates the path for the overlay.

