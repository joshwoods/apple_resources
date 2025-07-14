

- WatchKit
- WKInterfaceMap
-  setUserTrackingMode(\_:animated:) 

Instance Method

# setUserTrackingMode(\_:animated:)

Sets the map’s tracking mode.

watchOS 6.1+

``` source
func setUserTrackingMode(
    _ mode: WKInterfaceMap.UserTrackingMode,
    animated: Bool
)
```

## Parameters 

`mode`  

The desired tracking mode. For a complete list of valid tracking modes, see WKInterfaceMap.UserTrackingMode.

`animated`  

A Boolean value that indicates whether the map animates the change to the tracking mode.

## Discussion

By default, the tracking mode is WKInterfaceMap.UserTrackingMode.none.

Setting the tracking mode to WKInterfaceMap.UserTrackingMode.follow causes the map to center on the user’s location and begin tracking the user. If the map is zoomed out, the map view automatically zooms in on the user’s location, effectively changing the current visible region.

## See Also

### Displaying the User’s Location

func setShowsUserLocation(Bool)

Sets whether the map shows the user’s current location.

func setShowsUserHeading(Bool)

Sets whether the map shows the user heading.

enum UserTrackingMode

Modes for tracking the user’s location on the map.

