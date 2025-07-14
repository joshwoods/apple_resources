

- WatchKit
-  WKInterfaceMapPinColor 

Enumeration

# WKInterfaceMapPinColor

Constants for map pin colors.

watchOS

``` source
enum WKInterfaceMapPinColor
```

## Topics

### Constants

case red

A red pin.

case green

A green pin.

case purple

A purple pin.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Map Annotations

func addAnnotation(CLLocationCoordinate2D, with: UIImage?, centerOffset: CGPoint)

Displays the specified image on top of the map.

func addAnnotation(CLLocationCoordinate2D, withImageNamed: String?, centerOffset: CGPoint)

Displays an image from the WatchKit app’s bundle on top of the map.

func addAnnotation(CLLocationCoordinate2D, with: WKInterfaceMapPinColor)

Adds a pin to the map at the specified location.

func removeAllAnnotations()

Removes all annotations from the map.

