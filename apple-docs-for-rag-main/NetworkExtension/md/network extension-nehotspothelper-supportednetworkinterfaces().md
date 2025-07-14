

- Network Extension
- NEHotspotHelper
-  supportedNetworkInterfaces() 

Type Method

# supportedNetworkInterfaces()

Return the list of network interfaces managed by the Hotspot Helper infrastructure.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func supportedNetworkInterfaces() -> [Any]?
```

## Return Value

If no network interfaces are being managed, this function returns nil. Otherwise, an array of `NEHotspotNetwork` objects is returned.

## Discussion

Each network interface is represented by an NEHotspotNetwork object. Currently, the returned array contains exactly one NEHotspotNetwork object representing the Wi-Fi interface.

The main purpose of this method is to allow a Hotspot Helper to provide accurate status in its UI at times when it has not been given a command to process. This method coupled with the `isChosenHelper` method of NEHotspotNetwork allows the application to know whether it is the one that is handling the current network.

