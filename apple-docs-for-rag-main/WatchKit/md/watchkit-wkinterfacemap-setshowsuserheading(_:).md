

- WatchKit
- WKInterfaceMap
-  setShowsUserHeading(\_:) 

Instance Method

# setShowsUserHeading(\_:)

Sets whether the map shows the user heading.

watchOS 6.1+

``` source
func setShowsUserHeading(_ showsUserHeading: Bool)
```

## Discussion

By default, the map doesn’t show the user’s heading.

Note

Calling this method has no effect unless the map is showing the user’s location. For more information, see setShowsUserLocation(_:).

## See Also

### Displaying the User’s Location

func setShowsUserLocation(Bool)

Sets whether the map shows the user’s current location.

func setUserTrackingMode(WKInterfaceMap.UserTrackingMode, animated: Bool)

Sets the map’s tracking mode.

enum UserTrackingMode

Modes for tracking the user’s location on the map.

