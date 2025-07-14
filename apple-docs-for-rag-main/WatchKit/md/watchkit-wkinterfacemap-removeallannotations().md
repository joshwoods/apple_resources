

- WatchKit
- WKInterfaceMap
-  removeAllAnnotations() 

Instance Method

# removeAllAnnotations()

Removes all annotations from the map.

watchOS 2.0+

``` source
func removeAllAnnotations()
```

## See Also

### Managing Map Annotations

func addAnnotation(CLLocationCoordinate2D, with: UIImage?, centerOffset: CGPoint)

Displays the specified image on top of the map.

func addAnnotation(CLLocationCoordinate2D, withImageNamed: String?, centerOffset: CGPoint)

Displays an image from the WatchKit app’s bundle on top of the map.

func addAnnotation(CLLocationCoordinate2D, with: WKInterfaceMapPinColor)

Adds a pin to the map at the specified location.

enum WKInterfaceMapPinColor

Constants for map pin colors.

