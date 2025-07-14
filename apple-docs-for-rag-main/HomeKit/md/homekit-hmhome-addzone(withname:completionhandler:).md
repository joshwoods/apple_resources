

- HomeKit
- HMHome
-  addZone(withName:completionHandler:) 

Instance Method

# addZone(withName:completionHandler:)

Adds a new zone to the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func addZone(
    withName zoneName: String,
    completionHandler completion: @escaping (HMZone?, (any Error)?) -> Void
)
```

``` source
func addZone(named zoneName: String) async throws -> HMZone
```

## Parameters 

`zoneName`  

The name of the new zone. Must not be `nil`, and must not be the name of a zone already in the home.

`completion`  

The block executed after the request is processed.

zone  
The newly created zone.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Grouping rooms into zones

var zones: [HMZone]

An array of all the zones in the home.

func removeZone(HMZone, completionHandler: ((any Error)?) -> Void)

Removes a zone from the home.

class HMZone

A collection of rooms that users think of as a single area, like upstairs or downstairs.

