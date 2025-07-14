

- Network Extension
- NEHotspotNetwork
-  setConfidence(\_:) 

Instance Method

# setConfidence(\_:)

Indicate the level of confidence in being able to handle the network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setConfidence(_ confidence: NEHotspotHelperConfidence)
```

## Parameters 

`confidence`  

The level of confidence that the caller has in being able to help the system connect to this network.

## Discussion

Hotspot Helper apps use this method in the response to the NEHotspotHelperCommandType.evaluate and NEHotspotHelperCommandType.filterScanList commands.

## See Also

### Network annotation

enum NEHotspotHelperConfidence

A type that indicates the hotspot helper’s confidence in its ability to handle the network.

func setPassword(String)

Provide the password for a protected network.

