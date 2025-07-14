

- WatchKit
- WKInterfaceMap
-  setShowsUserLocation(\_:) 

Instance Method

# setShowsUserLocation(\_:)

Sets whether the map shows the user’s current location.

watchOS 6.1+

``` source
func setShowsUserLocation(_ showsUserLocation: Bool)
```

## Parameters 

`showsUserLocation`  

A Boolean value that indicates whether the map shows the user’s current location.

## Discussion

Setting this property to true displays the users current location on the map. The default value is false.

This property doesn’t indicate whether the user’s position is visible on the map. Setting this property to true causes the map view to use the Core Location framework to track the user’s current location and display the location when it’s visible on screen. To keep the map centered on the user’s location, pass WKInterfaceMap.UserTrackingMode.follow to the setUserTrackingMode(_:animated:) method.

## See Also

### Displaying the User’s Location

func setShowsUserHeading(Bool)

Sets whether the map shows the user heading.

func setUserTrackingMode(WKInterfaceMap.UserTrackingMode, animated: Bool)

Sets the map’s tracking mode.

enum UserTrackingMode

Modes for tracking the user’s location on the map.

