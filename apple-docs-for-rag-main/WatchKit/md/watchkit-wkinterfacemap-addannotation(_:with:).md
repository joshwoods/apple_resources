

- WatchKit
- WKInterfaceMap
-  addAnnotation(\_:with:) 

Instance Method

# addAnnotation(\_:with:)

Adds a pin to the map at the specified location.

watchOS 2.0+

``` source
func addAnnotation(
    _ location: CLLocationCoordinate2D,
    with pinColor: WKInterfaceMapPinColor
)
```

## Parameters 

`location`  

The location at which to display the pin.

`pinColor`  

The color of the pin. For a list of possible values, see WKInterfaceMapPinColor.

## Discussion

The pin is positioned so that the base of the pin sits on top of the specified coordinate.

## See Also

### Managing Map Annotations

func addAnnotation(CLLocationCoordinate2D, with: UIImage?, centerOffset: CGPoint)

Displays the specified image on top of the map.

func addAnnotation(CLLocationCoordinate2D, withImageNamed: String?, centerOffset: CGPoint)

Displays an image from the WatchKit app’s bundle on top of the map.

enum WKInterfaceMapPinColor

Constants for map pin colors.

func removeAllAnnotations()

Removes all annotations from the map.

