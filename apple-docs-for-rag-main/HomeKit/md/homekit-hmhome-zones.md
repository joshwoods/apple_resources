

- HomeKit
- HMHome
-  zones 

Instance Property

# zones

An array of all the zones in the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var zones: [HMZone] { get }
```

## See Also

### Grouping rooms into zones

func addZone(withName: String, completionHandler: (HMZone?, (any Error)?) -> Void)

Adds a new zone to the home.

func removeZone(HMZone, completionHandler: ((any Error)?) -> Void)

Removes a zone from the home.

class HMZone

A collection of rooms that users think of as a single area, like upstairs or downstairs.

