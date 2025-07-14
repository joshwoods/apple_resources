

- WatchKit
-  WKInterfaceMap 

Class

# WKInterfaceMap

An interface element that displays a noninteractive map for the location you specify.

watchOS 2.0+

``` source
class WKInterfaceMap
```

## Overview

You can configure Maps dynamically from your interface controller. Use the methods of WKInterfaceMap to specify the visible region of the map and to add any annotations or points of interest. Tapping the map launches the Maps app on the user’s Apple Watch and displays the corresponding location.

Using a map object, you specify a geographic region to display and you can optionally add annotations to the surface of the map. Maps display annotations as images on top of the map content. You can use custom images or display the built-in pin images. Maps can display no more than five annotations at a time.

Don’t subclass or create instances of this class yourself. Instead, define outlets in your interface controller class and connect them to the corresponding objects in your storyboard file. For example, to refer to a map object in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var myMap: WKInterfaceMap!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceMap* myMap;
```

During the initialization of your interface controller, WatchKit creates a new instance of this class and assigns it to your outlet. At that point, you can use the object in your outlet to make changes to the onscreen map.

The Apple Watch must have an active network connection to download map tiles.

### Configure the Map in Interface Builder

In Xcode, you can configure information about your map from your storyboard file. The map interface object has an Enabled attribute that appears as a checkbox in the Attributes inspector. When you enable the map interface object in this checkbox, tapping the map launches the Maps app and displays the current selected location.

## Topics

### Specifying the Map Region

func setVisibleMapRect(MKMapRect)

Changes the map’s visible region to the specified map rectangle.

func setRegion(MKCoordinateRegion)

Changes the map’s visible region to the specified coordinate region.

### Managing Map Annotations

func addAnnotation(CLLocationCoordinate2D, with: UIImage?, centerOffset: CGPoint)

Displays the specified image on top of the map.

func addAnnotation(CLLocationCoordinate2D, withImageNamed: String?, centerOffset: CGPoint)

Displays an image from the WatchKit app’s bundle on top of the map.

func addAnnotation(CLLocationCoordinate2D, with: WKInterfaceMapPinColor)

Adds a pin to the map at the specified location.

enum WKInterfaceMapPinColor

Constants for map pin colors.

func removeAllAnnotations()

Removes all annotations from the map.

### Displaying the User’s Location

func setShowsUserLocation(Bool)

Sets whether the map shows the user’s current location.

func setShowsUserHeading(Bool)

Sets whether the map shows the user heading.

func setUserTrackingMode(WKInterfaceMap.UserTrackingMode, animated: Bool)

Sets the map’s tracking mode.

enum UserTrackingMode

Modes for tracking the user’s location on the map.

### Initializing for SwiftUI

init()

Creates a map for use in SwiftUI.

Deprecated

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Controls

class WKInterfaceLabel

An interface element that displays static text.

class WKInterfaceDate

A label that displays the current date or time.

class WKInterfaceTimer

A label that displays a countdown or count-up timer.

class WKInterfaceButton

A button in the user interface of your watchOS app.

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

class WKInterfacePaymentButton

A button that you can use to trigger payments through Apple Pay.

class WKInterfaceTextField

An interface element that displays an editable text area.

class WKInterfaceSwitch

An interface element that toggles between an On and Off state.

class WKInterfaceSlider

An interface element that lets users select a single floating-point value from a range of values.

class WKInterfaceActivityRing

A view that displays data from a HealthKit activity summary object.

