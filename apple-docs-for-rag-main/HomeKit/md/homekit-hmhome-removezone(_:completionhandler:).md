

- HomeKit
- HMHome
-  removeZone(\_:completionHandler:) 

Instance Method

# removeZone(\_:completionHandler:)

Removes a zone from the home.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func removeZone(
    _ zone: HMZone,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func removeZone(_ zone: HMZone) async throws
```

## Parameters 

`zone`  

The zone to remove.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Grouping rooms into zones

var zones: [HMZone]

An array of all the zones in the home.

func addZone(withName: String, completionHandler: (HMZone?, (any Error)?) -> Void)

Adds a new zone to the home.

class HMZone

A collection of rooms that users think of as a single area, like upstairs or downstairs.

