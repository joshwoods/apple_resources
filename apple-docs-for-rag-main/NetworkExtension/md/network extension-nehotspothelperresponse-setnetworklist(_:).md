

- Network Extension
- NEHotspotHelperResponse
-  setNetworkList(\_:) 

Instance Method

# setNetworkList(\_:)

Set the list of handled networks.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setNetworkList(_ networkList: [NEHotspotNetwork])
```

## Parameters 

`networkList`  

The list of networks that the caller is capable of handling.

## Discussion

The Hotspot Helper app calls this method on its response to the NEHotspotHelperCommandType.filterScanList. The helper provides the list of network objects that it is capable of handling with at least low confidence. Networks that it has no confidence in handling should not be specified.

## See Also

### Response properties

func setNetwork(NEHotspotNetwork)

Set the network that conveys the confidence level.

