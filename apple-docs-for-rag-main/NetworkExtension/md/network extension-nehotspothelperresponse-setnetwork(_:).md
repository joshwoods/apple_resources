

- Network Extension
- NEHotspotHelperResponse
-  setNetwork(\_:) 

Instance Method

# setNetwork(\_:)

Set the network that conveys the confidence level.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setNetwork(_ network: NEHotspotNetwork)
```

## Parameters 

`network`  

The annotated NEHotspotNetwork object. This must be the same object that was passed in the corresponding NEHotspotHelperCommand object.

## Discussion

In response to the NEHotspotHelperCommandType.evaluate command, the Hotspot Helper app sets the confidence level on the NEHotspotNetwork object provided with the command and calls this method to convey the confidence level to the system.

## See Also

### Response properties

func setNetworkList([NEHotspotNetwork])

Set the list of handled networks.

