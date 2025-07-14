

- Network Extension
- NEHotspotNetwork
-  setPassword(\_:) 

Instance Method

# setPassword(\_:)

Provide the password for a protected network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setPassword(_ password: String)
```

## Parameters 

`password`  

The network password.

## Discussion

The Hotspot Helper may set a password for a protected network. The password string must adhere to IEEE 802.11 guidelines appropriate for the particular security scheme.

Hotspot Helper apps use this method only in the response to the NEHotspotHelperCommandType.filterScanList command.

## See Also

### Network annotation

func setConfidence(NEHotspotHelperConfidence)

Indicate the level of confidence in being able to handle the network.

enum NEHotspotHelperConfidence

A type that indicates the hotspot helper’s confidence in its ability to handle the network.

